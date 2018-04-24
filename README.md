# deezer-cli

## Introduction

deezer-cli is a command line interface to Deezer. It consumes the ability of AppleScript on OSX to send JavaScript commands to any Safari instance.

In the current setup Deezer is set as the second tab in Safari. Therefore, any command will target the second tab of the first Safari instance AppleScript will get hold on. The number of the tab can be changed in the deezer shellscript itself.

### Available commands

```
usage: deezer [--help] <command>

title       get title of Deezer window
goto        change url of Deezer window
activate    activate window if Deezer is not loaded yet. Will be run at every start.
track       get title of track
play        play track
pause       pause track
status      show status
next        play next track
prev        play previous track
usage       this message
```

### Example

```
$ deezer status
▶
$ deezer track
Motörhead - Shine
$ deezer pause
$ deezer status
◼
$ deezer next
$ deezer track
The Mars Volta - Televators
$ deezer play
$ deezer status
▶
$ deezer goto https://www.deezer.com/en/album/1206014
```
## Setup
You will have to explicitly grant the right of accessing web contents with JavaScript to AppleScript. This can be done by activating `Allow JavaScript from Apple Events` option in Safari.
