# deezer-cli

## Introduction

deezer-cli is a command line interface to Deezer. It consumes the ability of AppleScript on OSX to send JavaScript commands to any Safari instance.

In the current setup Deezer is set as the second tab in Safari. Therefore, any command will target the second tab of the first Safari instance AppleScript will get hold on.

### Available commands

```
deezer play
deezer pause
deezer next
deezer state
deezer title
deezer goto url
```

## Setup
You will have to explicitly grant the right of accessing web contents with JavaScript to AppleScript. This can be done by activating `Allow JavaScript from Apple Events` option in Safari.
