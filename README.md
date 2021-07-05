# KHPC-Music-Tools
Tutorial: https://www.youtube.com/watch?v=BnuQA9fDcog <br/>
Track Locations: https://docs.google.com/spreadsheets/d/1Z16-I8FbuVzXqCg0uhPkpvxeNz2xrJnA/edit#gid=1851343023
#### Music Encoder:
Converts WAV files to Kingdom Hearts PC music format <br/>
Use this for every track except KH1 Dive Into The Heart(music132.win32.scd)
##### Usage:
MusicEncoder <InputSCD/Dir> <InputWAV/Dir> [Quality] <br/>
Quality is an optional parameter that ranges from 0 to 10, by default is 10 <br/>
you can change it to reduce filesize, but that can interfere with custom loops
#### Multi Encoder:
Converts WAV files to Kingdom Hearts PC music format, use this for KH1 Dive Into The Heart(music132.win32.scd)
##### Usage:
MultiEncoder <InputSCD/Dir> [Quality] <br/>
Put the WAVs in the multiencoder folder <br/>
Rename them starting from 1.wav until you fulfil the number of tracks <br/>
In Dive Into The Heart the last one would be 8.wav <br/>
Quality is an optional parameter that ranges from 0 to 10, by default is 10 <br/>
you can change it to reduce filesize, but that can interfere with custom loops
#### How to Input Loops:
##### Full Loop:
WAV must have LoopStart and LoopEnd tags <br/>
LoopStart must be equal to 0 <br/>
LoopEnd must be equal to the last sample of the WAV.
##### Custom Loop:
WAV must have LoopStart and LoopEnd tags <br/>
LoopEnd must be equal to the last sample of the WAV.
##### No Loop:
WAV must not have LoopStart and LoopEnd tags.
#### Music Info:
Shows data from SCD files, decrypts them and extracts music files from them.
##### Usage:
MusicInfo info|extract|decrypt File/Dir
