---
layout: default
title: Week Nine
---

## Extracting Features

For this section I was required to extract Waveforms, Spectrograms, Mel Frequency Cepstral Coefficients and Chromagrams from three music tracks using Sonic Visualiser.

As my portfolio is based upon one specific song I have chosen to split it into three separate audio files using Audacity:

- Section One - 0s to 54s
- Section Two - 54s to 1m 40s
- Section Three - 1m 40s to end

I have split the file into three this way as each is a contrasting section of the piece, differing in tempo and key signature.

### Section One

<p float align="center">
    <img src="/data/Images/For Week Nine/KS Section One Waveform.png" width="900" />
    <img src="data/Images/For Week Nine/KS Section One Spectrogram.png" width="900" />
    <img src="data/Images/For Week Nine/KS Section One MFCC.png" width="900" />
    <img src="data/Images/For Week Nine/KS Section One Chromagram.png" width="900" />
</p>

### Section Two

<p float align="center">
    <img src="/data/Images/For Week Nine/KS Section Two Waveform.png" width="900" />
    <img src="data/Images/For Week Nine/KS Section Two Spectrogram.png" width="900" />
    <img src="data/Images/For Week Nine/KS Section Two MFCC.png" width="900" />
    <img src="data/Images/For Week Nine/KS Section Two Chromagram.png" width="900" />
</p>

### Section Three

<p float align="center">
    <img src="/data/Images/For Week Nine/KS Section Three Waveform.png" width="900" />
    <img src="data/Images/For Week Nine/KS Section Three Spectrogram.png" width="900" />
    <img src="data/Images/For Week Nine/KS Section Three MFCC.png" width="900" />
    <img src="data/Images/For Week Nine/KS Section Three Chromagram.png" width="900" />
</p>

## Histograms

For this section I was required to create Histograms for the features of the CSV files created from the audio files as shown above, in order to visualise differences between tracks in comparison to differences heard purely by listening.

### Histograms from Spectrograms

|Section One|Section Two|Section Three|
|--- |--- |--- |
| <img src="data/Images/For Week Nine/KS Section One Spectrogram Histogram.png" width="550" /> | <img src="data/Images/For Week Nine/KS Section Two Spectrogram Histogram.png" width="550" /> | <img src="data/Images/For Week Nine/KS Section Three Spectrogram Histogram.png" width="550" /> |

### Histograms from MFCCs

|Section One|Section Two|Section Three|
|--- |--- |--- |
| <img src="data/Images/For Week Nine/KS Section One MFCC Histogram.png" width="550" /> | <img src="data/Images/For Week Nine/KS Section Two MFCC Histogram.png" width="550" /> | <img src="data/Images/For Week Nine/KS Section Three MFCC Histogram.png" width="550" /> |

### Histograms from Chromagrams

|Section One|Section Two|Section Three|
|--- |--- |--- |
| <img src="data/Images/For Week Nine/KS Section One Chromagram Histogram.png" width="550" /> | <img src="data/Images/For Week Nine/KS Section Two Chromagram Histogram.png" width="550" /> | <img src="data/Images/For Week Nine/KS Section Three Chromagram Histogram.png" width="550" /> |

### Comparison of Histograms from Chromagrams

The chromagram's 12 functions relate to the twelve pitches of the chromatic scale (C C# D D# E F F# G G# A A# B), with time along the X axis and number of occurances along the Y axis.
This is useful when comparing how common pitches are across different audio files, and in the case of this analysis between the three sections of Кавал Свири.

One of the first comparisons that can be made is between sections one and two is the difference in harmony and amount of notes being sung at once. 
Section one is mostly in two part harmony with some four part towards the end, compared to section two which is entirely in four part harmony. We can see this in the Chromagram Histograms where there are more instances in section one around the notes of the Eminor chord (E G B) the melody moves around, compared to the more average distribution in section two as the melody and harmony develop.

However, there is an issue with this in the form of tuning in the recording, as the recording in question has the choir singing slightly flat when compared to the Western standard equal temperment with A=440Hz. This is due to the traditions and conventions of Bulgarian music being different.
Due to this, analysis must remember to look at both the note in question and the one a semitone below.

When contrasting the previous sections with section three, the main change is the shift from being predominantly in Eminor to Emajor. The clearest representation of this can be seen when comparing sections two and three as the most common occurances shift up one function as the key changes.

While these comparisons were able to be made on close inspection, they were not immediately obvious.