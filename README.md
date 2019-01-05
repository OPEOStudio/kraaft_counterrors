# kraaft_counterrors
A quick &amp; dirty python module + methodology to compare real text to what gspeech says

------------------------------------------------------------
METHODOLOGY

Two metrics - WER and SER

WER = (S + D + I ) / N

where :

S is number of substitutions (I surf small waves // I surf small awe)
D is number of deletions (I surf small waves // I surf waves)
I is number of insertions (I surf small waves // I surf small rider waves)
N is number of words total

SER = S(WER lower than 1) / S(total)

S sentences

Possible developments :

A. Identify intent (this is a wormhole)
B. Ponderate words
C. Include feedback from user (i.e number of repeats, ...)

------------------------------------------------------------
STRUCTURE

- takes two .json as inputs (a human and a automated) with list of sentences
- gives back two results : WER and SER

------------------------------------------------------------
THANKS & litterature

Relying heavily on :

https://en.wikipedia.org/wiki/Word_error_rate
http://blog.voicebase.com/how-to-compare-speech-engine-accuracy
https://www.quora.com/How-do-I-measure-the-accuracy-of-speech-recognition
https://medium.com/descript/comparing-the-accuracy-of-automatic-transcription-services-519fec134465
https://cds.cern.ch/record/2304470/files/report.pdf
