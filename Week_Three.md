---
layout: default
title: Week Three
---

Here is an inlined version of the Кавал Свири score via Verovio.

## Кавал Свири

{% include_relative Kaval_Sviri_verovio_inline.html %}

## Comparison of MusicXML and MEI

An important consideration to be taken when comparing MusicXML and MEI is that while they do have similarities they have two different goals, as specified on the [MEI Website](https://music-encoding.org/about/#:~:text=How%20is%20MEI%20different%20from,interchange%20format%20between%20notation%20editors.) - MusicXML is primarily focused on being interchangable between notation editors while MEI is primarily focused on the encoding of a scores notation and intellectual content.

1. One of the main differenes between MusicXML and MEI has to do with their ways of representing metadata.

   MusicXML has separate sections for the various metadata, such as `<work>` for the title, `<identification>` for the composer, arranger and encoding information, and a `<part-list>` for instrumentation including MIDI information.

   MEI on the other hand features all of this information within its `<meiHead>` which has sections for the same information able to be shown in MusicXML, however these are separated out into more distinct sections with conventions for referencing Authorities as well as more indepth encoding information.

   This makes the MEI appear more complex as it has more levels in which to display information.

2. Another difference that I noticed was within the descriptions of each individual instrumental/vocal part of the score
   Music XML lists the Part Name (with abbreviation), Instrument name (with abbreviation) and MIDI instrument information (including channel, program & volume.)

   MEI features the same information, as well as the additional information of the clef, key signature and time signature of each individual part.

   In addition to the difference in amounts of information tracked, the MEI file features a more condensed layout in terms of lines used, keeping all of the MIDI information under one `<instrDef>` line whereas MusicXML uses `<midi-instrument>` as a parent to several sub-sections.

   I find that this results in MEI being easier to read as types of information can be more clearly distinguished as they exist in one line each.

3. A third and rather large difference between MusicXML and MEI comes in relation to how measures and parts are represented and ordered within the text.

    MusicXML has each part as its own section, having for part one (`<part id="P1">`) be the parent for the entirety of that parts notes in the score, before closing the part and moving onto part two, and so on.

    On the other hand, MEI has the `<measure>` as the parent to the parts, describing each parts notes from top to bottom in a single measure before moving to the next measure and repeating the same process.

    This leads to MEI being closer to the reality of a music score, where all of the parts within one measure play before moving onto the next, resulting in it being easier to follow than MusicXML where each part of the score has its own entire section.