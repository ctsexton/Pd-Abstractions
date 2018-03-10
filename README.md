# Pd-Abstractions
Time saving Pure Data abstractions for building digital instruments quickly and easily.

sample_loader.pd: takes an argument for a path to a folder of audio samples and loads each of them into arrays. Samples are accessible in arrays named "1-sample, 2-sample... etc." REQUIRES: Cyclone library (specifically the counter object). Vanilla Pd version coming soon!

LaunchPatches: Novation products (Launchpad, Launchkey, LaunchControl) are mapped with MIDI numbers to address buttons. The buttons however are usually in a grid layout (borrowing from the monome grid). These abstractions allow the user to address the grid buttons as X/Y coordinates, making it far easier to isolate specific columns or rows (or even diagonals) of the grid. It is far easier and quicker to build customised mappings of the grid this way - and also adapt existing monome applications to the Launchpad.

enc_to_range.pd: For use with Rotary Encoders or any other incremental encoder. Takes an input (positive/negative increments of 1) and creates a virtual slider between 0 and 1. You can set the number of steps in between 0 and 1 in order to adjust the resolution. Requires: list-abs library.
