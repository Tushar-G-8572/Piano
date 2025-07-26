# 🎹 Piano Keyboard Web App

This is a simple interactive piano keyboard built with **HTML, CSS, and JavaScript**. Users can play sounds by either **pressing keys on their keyboard** or **clicking the on-screen keys**. Each key is mapped to a corresponding `.mp3` audio file to simulate piano sounds.

---

## 🔑 Features

- Keyboard-to-sound mapping (`0-9` and `a-g`)
- Clickable UI keys with animation
- Real-time audio playback
- Active key highlighting with animation effect
- Clean and minimal front-end experience

---

## 🛠️ Technologies Used

- HTML5  
- CSS3  
- Vanilla JavaScript

---

## 🧠 How It Works

```js
// Object that maps key presses to corresponding audio files
let keyPiano = {
    "1": 'audio/1.mp3',
    "2": 'audio/2.mp3',
    "3": 'audio/3.mp3',
    ...
    "g": 'audio/g.mp3'
};

// Play sound on keydown
document.addEventListener('keydown', (event) => playPiano(event.key));

// Play sound on button click
keys.forEach(key => {
    key.addEventListener('click', () => {
        playPiano(key.dataset.key);
    });
});
