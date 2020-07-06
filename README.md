# jsfx-dsp
Set of plugins/libraries to help in manipulating audio in a DAW.

## Gain unity
Tool that compensates for volume difference after a signal processing that may have change the volume (typically equalization, distortion, compression).
Volume difference is detected as perceived loudness difference in LUFS.

Two modes are available :
- short-term adapting volume, for tone adjustment exploration
- integration for definitive and accurate volume adjustment when the signal processing doesn't change

######TODO
- Implement smart sample size auto-adjustment in function of compensation stability


## CompUnifier
This plugin is close to an usual compressor in resulting processing. Its particularities are its smart auto-setup abilities.

There is no threshold to set, no attack time, no release time, no output volume (automatically compensated).

The only setting are the ratio/mix, and very visual attack/sustain ranges. A graphical visualizer helps to set very easily the ranges around the signal transients.


######TODO
- Eliminate distortion that occurs on slow signal wave oscillations
- Finish the volume auto-compensation when everything else will be ok
- Draw in visualizer the resulting changes