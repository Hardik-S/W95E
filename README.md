# W95E

W95E is a single-page Windows 95 style browser demo with a voice-controlled cursor. The page renders a desktop, taskbar, selectable icons, a status window, and an instruction panel from `index.html`.

## How to Run

Open `index.html` in a modern desktop browser. The demo uses the Web Speech API, exposed as `SpeechRecognition` or `webkitSpeechRecognition`, so voice control works best in browsers that support that API and have microphone permission enabled.

## Controls

1. Press `Spacebar` to start listening.
2. Speak a movement command in the form `up 50`, `down 100`, `left 25`, or `right 75`.
3. Say `click` to select whatever desktop icon is under the simulated cursor.

The status window shows whether recognition is ready or listening, the last command heard, the cursor position, and a running command log.

## Current Desktop Actions

- `Recycle Bin` can be selected by moving the cursor over it and saying `click`.
- `kabir.txt` can be selected the same way and logs a short file-open message.

## Browser Support Notes

If the browser does not provide the Web Speech API, the page still loads but reports that speech recognition is not supported. In that case, use a browser with speech recognition support or add a keyboard/manual command fallback before relying on the demo for a presentation.
