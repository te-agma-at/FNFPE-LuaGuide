# DIALOGUES AND CUTSCENES
### Speakin' Something Up
In this tutorial, I will guide you through some functions for Dialogues and Cutscenes

## Cutscene/Dialogue Functions: "startDialogue(dialogueFile:String, song:String = null)"
Starts a dialogue loading a file inside `mods/data/your-song-name/`.

- `dialogueFile` - .TXT file to load
- `song` - Optional value for a Background music during the dialogue
Example: If i want to load a dialogue file `mods/data/bopeebo/dialogue.txt` using the pause menu song (Breakfast), i should use: `startDialogue('bopeebo/dialogue', 'breakfast')`

NOTE: When the dialogue is ended, it calls `startCountdown()`

NOTE 2: `onNextDialogue(line)` callback is called for every dialogue line passed

Dialogue is actually very useful for cutscenes!

## Cutscene/Dialogue Functions: "startVideo(videoFile:String)"
Starts a Video Cutscene

- `videoFile` - File name of your video, it must be inside `mods/videos/`

Example: If you wanted to start the video `mods/videos/ughCutscene.mp4`, you'd have to use `startVideo('ughCutscene')`

Just like Dialogue, it is also very useful

## Extra Stuff
### startCountdown(): Starts a countdown manually
### endSong(): Ends the song manually
These functions are just in case you forced a countdown stop/ending for a post/pre-song cutscene
