---
layout: post
title: 90SP - Vocal Cleanup
date: 2025-05-20 11:42:00 +0000
tags: 
  - music
  - technology
---

Here's my method that I've been using to cleanup vocals on the 90 songs project.

1. Auto-Align vocals to overhead R. This overhead is the main one, positioned directly over the snare. The snare has already been aligned to the overhead during recording.
2. De-bleed - first using the snare track to help with the transient of the snare, then with the overhead to help with cymbal bleed. The goal here isn't to completely remove the bleed, but to instead try and smear it back, allowing the vocal to be the predominant element in the recording.
3. De-plosive -  No idea how this works, but it really helps get rid of kick bleed. It's significantly better sounding than de-bleeding against the kick track.
4. Dialogue Isolate - Again, trying to follow that idea of pushing bleed into the background rather than getting rid of it completely. About -3dB down on the noise slider helps push back any remaining spill. I've pushed it up to -6dB down before getting artifacting, especially on the recordings where the vocalist has held the microphone rather than leaving it on a stand, making auto-aligning impossible.
5. Music Rebalance - I use this to solo just the vocal track, this is temporary so I use the lowest quality setting
6. Leveller - by using RX's leveller on the isolated vocal, I can get a really clean clip-gain curve that isn't trying to bring up any remaining spill. I can then copy the clip-gain information, revert back to the pre-rebalance version and paste it back

In some cases I've needed to go in and de-wind a few takes. I'll run this on the problematic parts rather than run it through the entire thing, as I've found it can lead to weird artifacts.

This method leaves me with vocal tracks that are isolated enough to do some light pitch correction with Melodyne or AutoTune, if needed! Not bad considering the vocalists were stood directly in front of a drum kit!