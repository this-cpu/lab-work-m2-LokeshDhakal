## Title:  MIDI Note Processing & Algorithmic Music Generation

## Objectives:

1. Print MIDI Channels, Notes & their Frequencies.
2. Create beat, harmony and melody using MIDI Notes.
3. Play the individual MIDI track (Mid File).
4. Combine the beat, harmony and melody in a single file.
5. Convert the MIDI tracks into the standard audio (.wav) file.

## Background Theory

- MIDI Standard
  1. Notes
  2. Frequency
     
- Music Theory
  1. Beat
  2. Harmony
  3. Melody
    
## Procedure

- Mido
- Pygame

This experiment was carried out using Python libraries including MIDO, pygame, and PyDub to perform MIDI note processing and algorithmic music generation. MIDI note numbers ranging from 69 to 127 were mapped to their corresponding note names and octaves using the formula octave = (midi_num // 12) - 1, following the MIDI standard where middle C (C4) corresponds to MIDI note 60. Three separate MIDI tracks were created by initializing individual MidiFile and MidiTrack objects: the beat track used percussion notes (kick drum, snare, hi-hat) arranged rhythmically with 480 ticks per beat; the harmony track generated chord progressions (Cmaj7, Gsus4, Am7, Fmaj7) by playing multiple notes simultaneously; and the melody track created a sequential phrase using eight notes repeated twice. Musical timing was controlled using tick values, while note duration and intensity were managed using note_on and note_off messages with specified velocities.

Each MIDI track was saved as a separate .mid file and played individually using the pygame mixer to verify timing and pitch accuracy. Finally, the individual tracks were converted to audio format and combined using PyDub. The beat and harmony tracks were looped to match the melody length using multiplication operations, trimmed accordingly, and overlaid using the overlay() method to produce a complete composition. The final mixed output was exported as a standard .wav file, successfully achieving all stated objectives including MIDI note processing, multi-track composition, individual playback verification, track combination, and audio format conversion.

## Output

The experiment successfully generated MIDI note mappings displaying MIDI numbers (69-127) with their corresponding note names and octaves in a formatted table. Three individual MIDI files were created and saved: beat.mid containing the percussion pattern with kick, snare, and hi-hat sounds; harmony.mid with chord progressions (Cmaj7, Gsus4, Am7, Fmaj7); and melody.mid with a 16-bar melodic phrase. Each track was successfully played back using pygame mixer, confirming proper timing and pitch accuracy.
The final combined composition was exported as final_song_pydub.wav, integrating all three tracks into a cohesive musical piece. The beat and harmony loops were properly synchronized with the melody length, and the overlay mixing preserved the individual characteristics of each track while creating a balanced overall sound. The output .wav file was playable in standard audio players, confirming successful conversion from MIDI to standard audio format.
