# Running the piano program(s)


## View help menu
```bash
java -jar PianoController.jar --help
```

## Running the main program
```bash
java -jar PianoController.jar run-server
```

## SongDB Verification
```bash
java -jar PianoController.jar songdb-verification
```
As a GitHub action:
```bash
java -jar PianoController.jar songdb-verification --github-action
```

## Midi Viewer
Show original midi file:
```bash
java -jar PianoController.jar midi-viewer -f <path-to-midi-file>
```

Show cleaned up midi file:
```bash
java -jar PianoController.jar midi-viewer -f <path-to-midi-file> --showCleanedOnly
```

Show original midi file and cleaned up midi file:
```bash
java -jar PianoController.jar midi-viewer -f <path-to-midi-file> --showOrigAndCleaned
```
## Key Debug
```
java -jar PianoController.jar key-debug
```

## Mapping Generator
```bash
java -jar PianoController.jar mapping-generator
```

## Midi Keyboard
```
java -jar PianoController.jar midi-keyboard
```
