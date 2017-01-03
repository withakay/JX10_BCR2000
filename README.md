# JX10 BCR2000

Here you will find sysex files and the source BCL scripts to configure a Behringer BCR2000 as an editor for the Vecoven upgraded Roland JX10. I have OS v3.03, I expect modifications will be required for these scripts to work with v4+

# Setup

Send the sysex files to your BCR (I use Elektron C6 for this, but there are plenty of options out there)

* Send jx10_upper_tone.syx to Preset 1
* Send jx10_lower_tone.syx to Preset 2
* Send jx10_both_tones.syx to Preset 3

Your JX10 should be set to use midi channel 1, for simplicity set upper, lower and control channels to 1
The script uses NRPNs and as such does not require sysex to be enabled, but you do need to set TONE CC = TRUE and I would recommend setting EDIT DISPLAY = SYSEX (which confussingly also relates to NRPNs in this case) as this will enable you to see what value is being edited when you twist an encoder.

Plug the BCR midi out to JX midi in and vice versa for bidirectional control.

The parameters are mapped thusly, but if you have taken my advice regarding EDIT DISPLAY simply movinging an encoder should make the JX10 display the currently edited parameter.

## ENVELOPES

To access ENV-1 parameters enable encoder group 1

* Encoder 1 ENV-1 Attack
* Encoder 2 ENV-1 Decay
* Encoder 3 ENV-1 Sus
* Encoder 4 ENV-1 Rel
* Encoder 5 Env1 Key Follow 4 positions
* Encoder 6 LFO Waveform 3 positions
* Encoder 7 LFO Speed
* Encoder 8 LFO Delay

To access ENV-2 parameters enable encoder group 2

* Encoder 9 ENV-2 Attack
* Encoder 10 ENV-2 Decay
* Encoder 11 ENV-2 Sustain
* Encoder 12 ENV-2 Rel
* Encoder 13 ENV-2 Key Follow
* Encoder 14 LFO Waveform Duplicate 3 positions
* Encoder 15 LFO Speed Duplicate
* Encoder 16 LFO Delay Duplicate

## OSCILLATORS

* Button 41 DCO-1 Octave 4 positions
* Button 42 DCO-1 Waveform 4 positions
* Button 43 not used
* Button 44 DCO-2 Octave 4 positions
* Button 45 DCO-2 Waveform 4 positions
* Button 46 DCO Crossmod 4 positions
* Button 47 DCO Dynamics 4 positions
* Button 48 DCO Env Mode 4 positions

* Encoder 33 DCO-1 Tune
* Encoder 34 DCO-1 LFO Level
* Encoder 35 DCO-1 Pitch Env
* Encoder 36 DCO-2 Tune
* Encoder 37 DCO-2 LFO Level
* Encoder 38 DCO-2 Pitch Env
* Encoder 39 DCO-2 Fine Tune
* Encoder 40 Chorus Mode 3 positions

## FILTERS

* Encoder 41 VCF Hi Pass 4 positions
* Encoder 42 VCF Freq
* Encoder 43 VCF Q
* Encoder 44 VCF LFO
* Encoder 45 VCF Env
* Encoder 46 VCF Key Follow
* Encoder 47 VCF Dynamic 4 positions
* Encoder 48 VCF Env Mode 4 positions

## MIXER

* Encoder 49 Level DCO-1 
* Encoder 50 Level DCO-2 
* Encoder 51 VCA Envelope Mod
* Encoder 52 VCA Dynamics 4 positions
* Encoder 53 VCA Env Mode 4 positions
* Encoder 54 VCA Base Level
* Encoder 55 VCA Dynamics 4 positions
* Encoder 56 VCA Gate/Env 2 positions

