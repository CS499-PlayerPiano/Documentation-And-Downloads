# Configuration

## Outputs.json
```json5
{
    // Configuration for the Logger output
    "Logger": {
        "enabled": true
    },

    // Configuration for the Midi Synthesizer
    "Midi Synthesizer": {
        "enabled": true
    },

    // Configuration for the Virtual Piano GUI
    "Virtual Piano GUI": {
        "enabled": true,

        // Either "RAINBOW_GRADIENT" or "TRACK_NUMBER"
        "colorMode": "RAINBOW_GRADIENT"
    },

    // Configuration for the Synthesia Viewer (Not yet implemented)
    "Synthesia Viewer": {
        "enabled": false
    },

    // Configuration for the web server
    "Javalin Web Server": {

        // Port to run the web server on
        "port": 8898,

        // Interval in milliseconds to send timestamp updates to the client
        "timestampInterval": 500
    },

    // Configuration for the Physical Piano
    "Arduino": {
        "enabled": true,

        // COM port for the Arduino
        "comPort": "COM7",

        // Baud rate for the Arduino
        "baudRate": 115200,

        // Should we print debug output if the Arduino sends it?
        "printDebugOutputFromArduino": true,

        // Should we send a power reset after every song?
        "sendPowerResetAfterEverySong": true,

        // Shoud we ignore velocity, and only send 255 or 0?
        "ignoreVelocity": false,

        // Velocity mapping for energising the solenoids.
        // The solenoids stop responding at 120, and are fully energised at 255.
        "velocityMapping": {
            "min": 120,
            "max": 255
        },

        // Mapping of the notes to the solenoids
        // Physical Key Index -> Midi Note
        // 0 is the lowest key, 87 is the highest key
        "noteMapping": {
            "0": 101,
            "1": 102,
            "2": 103,
            "3": 104,
            "4": 105,
            "5": 106,
            "6": 107,
            "7": 108,
            "8": 93,
            "9": 94,
            "10": 95,
            "11": 96,
            "12": 97,
            "13": 98,
            "14": 99,
            "15": 100,
            "16": 85,
            "17": 86,
            "18": 87,
            "19": 88,
            "20": 89,
            "21": 90,
            "22": 91,
            "23": 92,
            "24": 77,
            "25": 78,
            "26": 79,
            "27": 80,
            "28": 81,
            "29": 82,
            "30": 83,
            "31": 84,
            "32": 69,
            "33": 70,
            "34": 71,
            "35": 72,
            "36": 73,
            "37": 74,
            "38": 75,
            "39": 76,
            "40": 61,
            "41": 62,
            "42": 63,
            "43": 64,
            "44": 65,
            "45": 66,
            "46": 67,
            "47": 68,
            "48": 53,
            "49": 54,
            "50": 55,
            "51": 56,
            "52": 57,
            "53": 58,
            "54": 59,
            "55": 60,
            "56": 45,
            "57": 46,
            "58": 47,
            "59": 48,
            "60": 49,
            "61": 50,
            "62": 51,
            "63": 52,
            "64": 37,
            "65": 38,
            "66": 39,
            "67": 40,
            "68": 41,
            "69": 42,
            "70": 43,
            "71": 44,
            "72": 29,
            "73": 30,
            "74": 31,
            "75": 32,
            "76": 33,
            "77": 34,
            "78": 35,
            "79": 36,
            "80": 21,
            "81": 22,
            "82": 23,
            "83": 24,
            "84": 25,
            "85": 26,
            "86": 27,
            "87": 28
        }
    }
}
```

## Programs.json
```json5
{
    // Configuration for the Midi Keyboard Input
    "midi-keyboard": {
        // Should we print all the device names on boot?
        "printAllDeviceNames": true,

        // Name of the device to use
        "deviceName": "AKM320",

        // Should we ignore velocity when reading the midi input?
        "ignoreVelocity": true
    }
}
```

## TODO Configs:
We ran out of time to make these configurable, but they should be configurable in the future.
```
plu.capstone.playerpiano.sheetmusic.cleaner.steps.Step4OffsetNoteTimes LN: 28-120. timeToRelease(), timeToHit(), calcShiftForwardAmount()
```