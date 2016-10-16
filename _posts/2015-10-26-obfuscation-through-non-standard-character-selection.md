---
layout: post
title: Obfuscation Through Non-Standard Character Selection
date: 21-07-2016
categories: security thinks
author: HeadCrash
---
# Obfuscation Through Non-Standard Character Selection

> Here's a really shoddy attempt at hiding what you is ritINgs

There’s been a lot of discussion about obfuscation, cryptography and steganography and the like over the last week or so here in the FU:Comp bunker. Various methods of encryption, obfuscation and diverse other ways of futzing with Big Bother came up but this one floated to the surface as standing out as having some fairly interesting points.

What we’re trying to achieve here is the most basic way possible of preventing automated systems from reading your text. What we are definitely not trying to do here is show anyone how to make it impossible for outside agents to access your sensitive data.

I took the following phrase from the Hacker’s Manifesto as archived in Phrack Magazine #07 from ’96.

I am a hacker, and this is my manifesto. You may stop this individual, but you can’t stop us all… after all, we’re all alike.
I then ran it through the open-sourced online text mangler at Lunicode using the “bent” method which then spat out:

```
į ąʍ ą հąçҟҽɾ, ąղժ էհìʂ ìʂ ʍվ ʍąղìƒҽʂէօ. Ӌօմ ʍąվ ʂէօք էհìʂ ìղժìѵìժմąӀ, ҍմէ վօմ çąղ’է ʂէօք մʂ ąӀӀ… ąƒէҽɾ ąӀӀ, աҽ’ɾҽ ąӀӀ ąӀìҟҽ.
```
Note that you’ll need a unicode font installed to see this.

Then I took a screenshot of the textbox and sent it through an OCR converter. I’m only displaying the best result I got because Google Docs just could not even and others just returned blank files.

### Obfuscated text before OCR
![Obfuscated text before OCR](http://media.fuckyou.computer/pre-ocr.png)

### Deobfuscated text via OCR
![Obfuscated text via OCR](http://media.fuckyou.computer/post-ocr.png)

As you can see it’s not perfect but it’s broken up enough of the meaning that I think a cursory scrape wouldn’t pick up anything of note.

## Key:

NFI – Computer didn’t even get anywhere close so this is essentially just noise.
Correct – Computer guessed this word.
Incorrect – Computer guessed this word incorrectly.
Incorrect – Computer guessed this word also incorrectly but was close.

```
1 am a mafia, aqd tcis is M4 Maqifesto. bled M214
Stop this individaal, 13;“;qu caq’l; stop as all… after
all, we’re all alike.
```

This method is intended for person to person use only, it’s incredibly easy for someone to glance at the text and read it but currently impossible for a computer to grasp the context and therefore meaning of a conversation it may have intercepted.

This could be made stronger by adding nonsense words into your written vocabulary, using some sort of shorthand like 13375934k or using multiple levels of the same technique.

Using a dictionary spellchecker and matching against the most likely word probably would have netted the computer the correct matches for “Maqifesto” and “individaal” so that’s a thing to be wary of.

## Pros:

* Mostly resistant to OCR.
* Definitely resistant to automated content searches as long as point 1 remains true.
* Easily read by humans.

## Cons:

* Resistant to searches. You’re going to want to remember where you parked your documents, kids. And already know what’s in them.
* Easily read by humans, even those who you don’t know are looking. Over your shoulder, say.
* Lunicode is bidirectional


## Useful links

* Lunicode.com
* Online OCR
* The Hacker Manifesto
