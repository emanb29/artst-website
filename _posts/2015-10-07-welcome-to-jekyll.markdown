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
In order to [harvest the energy from (and provide security while) walking](https://blog.mide.com/piezoelectric-energy-harvesting-from-walking), we opted to [install piezoelectric cells into the shoes wired to illuminate LEDs](http://www.instructables.com/id/Electricity-Generating-Footwear/), as well as mount retroreflective plating on the sides of the shoes (the material street signs are made of). Ideally, this will be a simple enough construction that a commercial kit could be made to apply to your existing shoes.

## Challenges
There were several challenges to overcome, each detailed below:

### Generating power
In order to effectively generate power, we not only needed to find efficient piezoelectric cells, but also optimally place those cells. Unfortunately, the first batch of piezoelectric cells we ordered were incredibly frail and produced too little current to be usable. They did, however, have way higher voltage output than expected.
![Typical voltage rating from old piezo cells at 15 degree bend](https://i.imgur.com/4cceLfh.jpg)
### Converting power to a usable form
Piezo cells generate an incredibly inconsistent, very high-voltage, and astonishingly low-current AC flow of electricity. While inconsistency is fine (and might even be to the benefit of flashing LEDs), without a strong electrical engineering background, we were uncertain of the implications of high-voltage and low-current power. What we did figure out, rather quickly, is how to convert low-power AC current into low-power DC current without major loss (since LEDs only work with DC current). For this purpose, we made a simple circuit called a bridge rectifier, consisting of four diodes.
![Diodes assortment](https://i.imgur.com/01Mf9A5.jpg)
![Power Conversion Circuit](https://i.imgur.com/LbjEyyJ.jpg)
Actually constructing these circuits proved to be a bit of an ordeal in itself, due to neither of us having much soldering experience (left example), but we eventually [found a solution that resulted in a much smaller and more sturdy final product (right example)](https://youtu.be/Fztzn2LcGOE?t=1m38s).
### Illuminating LEDs
Without much EE knowledge, as mentioned, we were unsure of how successful we would be in illuminating LEDs with high-voltage and low-current power. However, from some preliminary research, it seems that voltage is usually the limiting factor rather than amperage. Further, we found many sources (eg [here](http://lednique.com/current-voltage-relationships/iv-curves/) and [here](https://reefbuilders.com/2010/09/30/philips-lumileds-luxeon-rebel-color-leds-power/)) suggesting that red LEDs are *far* more current-efficient than other colors. As such, that is wwhat we ordered.

## Next Steps
To continue the project, there are a few avenues we will need to explore:
- Finding and rating better piezoelectric cells: We have ordered a few more piezo cells of different types. As datasheets seem incredibly hard to come by, we will have to rate the piezo cells ourselves, but luckily this is a simple and familiar process
- Testing LEDs: While the numbers don't look good for a single piezo cell being able to power an LED, we have so far only rated trashy (as mentioned) piezo cells, and in our final product, we'll be wiring a bunch of bridge-rectified (to avoid interference) cells in series for a much larger current.
- Carving the shoe: We need to find a place we can actually fit the electronics in the shoe. We chose some thick-soled shoes in the hopes that we will be able to carve a hole into the sole in which to place the electronics while retaining comfort.
- Applying retroreflective plating: This should actually be easy -- we found retroreflective tape for a great price!