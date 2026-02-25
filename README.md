# 🎂 AI Birthday Surprise Vault (生日惊喜大挑战)

A hilarious, interactive, AI-powered web application built to roast and celebrate a friend's birthday. This project uses computer vision to track facial landmarks and hand gestures in real-time directly within a mobile or desktop web browser. 

Instead of a boring birthday text, the user is forced to wear a live "clown" filter and complete embarrassing physical poses to unlock their birthday greeting—while the app secretly takes photos of them and downloads them to their device. 😈

## ✨ Features

* **Real-Time AI Tracking:** Utilizes Google's MediaPipe (FaceMesh & Hands) for high-performance tracking directly in the browser.
* **"IG-Style" Live Filter:** Automatically maps a transparent clown wig/nose PNG onto the user's face using dynamic landmark coordinates.
* **Gesture Recognition Engine:** * ✌️ **Stage 1:** Detects the "Peace" sign (index/middle fingers up, others down).
    * 👂 **Stage 2:** Detects hands placed over the ears.
* **Auto-Photo Booth:** Triggers a cinematic "white flash" and silently downloads high-quality screenshots (clown filter included!) to the user's device when they hold a pose.
* **Animorphs Crossfade Transition:** Smoothly morphs the live camera feed into premium meme images upon completing a stage.
* **100% Client-Side:** No backend required. Runs purely on HTML5 Canvas and JavaScript, making it perfect for free hosting and immediate mobile access.

## 🛠️ Tech Stack

* **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
* **Computer Vision / AI:** [MediaPipe for Web](https://google.github.io/mediapipe/) (`@mediapipe/hands`, `@mediapipe/face_mesh`, `@mediapipe/camera_utils`)
* **Rendering:** HTML5 `<canvas>` API
* **Deployment:** Vercel / GitHub Pages

## 📂 File Structure

To run this project, you need the following files in the same directory:

```text
├── index.html       # The main application engine and UI
├── clown.png        # Transparent overlay for the face filter
├── monke.jpg        # Meme asset for Stage 1 completion
├── teat1.jpg        # Meme asset for Stage 2 completion
└── bgm.mp3          # Looping background music
