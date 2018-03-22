---
layout: post
title: Safety Shoes - Spring Break Milestone
date:
  'Tue Mar 20 2018 17:00:00 GMT-0700 (Pacific Daylight Time)': null
preview: 'https://i.imgur.com/cFQgKA3.jpg'
published: true
---

![Parts Assembled](https://i.imgur.com/cFQgKA3.jpg)

## Motivation
In thinking about and doing research on sustainability, I discovered, espescially in the Portland area, people are exceptionally aware and conscious of sustainability in their personal lives, and try to factor it into their decisions. Where people feel they don't have the power to be more sustainable is at work. I wanted to address this.
### The Problem
Many people, espescially in big cities like Portland or small but relatively urbanized towns like Forest Grove, live within a mile or less of their workplace. Despite this, they tend to commute by car, a very unsustainable practice. One large reason for this is because the nights come so early in Oregon, people can be concerned about visibility to cars as they walk. Also, a lot of energy is wasted while walking in the form of shock. This extra vibration we generate is energy that doesn't serve us, and in fact can, over time, cause physical damage to our bodies.

## Concept
In order to harvest the energy from (and provide security while) walking, we opted to install piezoelectric cells into the shoes wired to illuminate LEDs, as well as mount retroreflective plating on the sides of the shoes (the material street signs are made of).

## Challenges
There were several challenges to overcome, each detailed below:

### Generating power
In order to effectively generate power, we not only needed to find efficient piezoelectric cells, but also optimally place those cells. Unfortunately, the first batch of piezoelectric cells we ordered were incredibly frail and produced too little current to be usable. They did, however, have way higher voltage output than expected.
![Typical voltage rating from old piezo cells at 15 degree bend](https://i.imgur.com/4cceLfh.jpg)
### Converting power to a usable form
Piezo cells generate an incredibly inconsistent, very high-voltage, and astonishingly low-current AC flow of electricity. While inconsistency is fine (and might even be to the benefit of flashing LEDs), without a strong electrical engineering background, we were uncertain of the implications of high-voltage and low-current power. What we did figure out, rather quickly, is how to convert low-power AC current into low-power DC current without major loss. For this purpose, we made a simple circuit called a bridge rectifier, consisting of four diodes.
![Power Conversion Circuit](https://i.imgur.com/LbjEyyJ.jpg)
Actually constructing these circuits proved to be a bit of an ordeal in itself, due to neither of us having much soldering experience (left example), but we eventually found a solution that resulted in a much smaller and more sturdy final product (right example).
### Illuminating LEDs

## Next Steps
To continue the project, there are a few avenues we will need to explore:
- Finding and rating better piezoelectric cells: We have ordered a few more piezo cells of different types. As datasheets seem incredibly hard to come by, we will have to rate the piezo cells ourselves, but luckily this is a simple and familiar process
- 