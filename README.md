# Deep-Audio-Isolation
Deep Audio Isolation: Isolating Vocals from Complex Musical Tracks.

Given an audio recording consisting of many mixed tracks (e.g vocals, instruments, background), it is often desirable to isolate one or more of those tracks individually. This has clear applications in fields like music/video-production, where it is useful to adjust individual tracks from a composite.

Generalising, the same capability could be applied to broader domains - such as active noise cancellation (or even augmentation), or as a pre-processing step to video-calls, voice-assistants, etc.

This problem is complicated because component tracks overlap in time and frequency. Thus, there is no analytic way to isolate them from each-other.  Historically, statistical techniques such as ICA have been used, and recently a wide array of CNN and RNN based approaches have risen.

As such, given a source-track containing several instruments, vocals, etc, a deep-learning model is proposed to extract a specific component track. While the architecture used is technically agnostic to the specific type of track isolated (e.g vocal, guitar, piano), we've focused our efforts on vocal isolation specifically.
