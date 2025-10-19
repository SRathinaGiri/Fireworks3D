# 3D Interactive Diwali Fireworks Show

A festive, web-based, and interactive 3D fireworks simulation built with **Three.js** to celebrate Diwali. This project features a dynamic fireworks display, a customizable 3D golden message, real-time effect controls, and video recording capabilities.

## Features

  * **Dynamic 3D Fireworks**: A beautiful, physics-based particle system that generates a wide variety of fireworks:
      * Standard & Multi-Color Bursts
      * Multi-Layer Ring Bursts
      * Cracking Cluster Bursts
      * Sparkler Fountains
      * Ground Spinners (Chakkars)
  * **Customizable 3D Message**: Display any message you like as beautiful, shining 3D golden text.
  * **Multi-Language Support**: By default, it uses an English font. You can provide your own custom font file (`FavLang.json`) to display messages in other languages like Tamil, Hindi, etc.
  * **Interactive Controls**:
      * Full camera control to zoom and rotate the scene.
      * Real-time sliders to control animation speed (slow-motion), blur/glow amount, and the number of fireworks.
      * Dynamically resizable canvas.
  * **Stereoscopic 3D**: Enable a side-by-side stereoscopic view, compatible with VR headsets or cross-eyed/parallel viewing techniques.
  * **Video Recording**: Record your custom fireworks show and download it as a `.webm` video file.

-----

## How to Run

If you need to give only English message you can run from the github page https://srathinagiri.github.io/Fireworks3D/

Because this application loads local files (`FavLang.json`), it needs to be run from a **local web server** due to browser security policies. Simply opening the HTML file from your file system (`file:///...`) will not work.

Here are two easy ways to start a local server:

### Method 1: VS Code with Live Server (Recommended)

1.  Install the **Live Server** extension by Ritwick Dey in Visual Studio Code.
2.  Open your project folder in VS Code.
3.  Click the **"Go Live"** button in the bottom-right corner of the window.

### Method 2: Python's Built-in Server

1.  Open a terminal or command prompt.
2.  Navigate to your project folder using the `cd` command.
3.  Run the following command:
    ```bash
    python -m http.server
    ```
4.  Open your browser and go to `http://localhost:8000/your_file_name.html`.

-----

## Controls & Usage

  * **Mouse**: Click and drag to rotate the camera. Use the scroll wheel to zoom in and out.
  * **Message**: Type your custom message before it appears (it appears after 15 seconds).
  * **Use Custom Font**: Check this box to switch from the default English font to your `FavLang.json` file.
  * **Canvas Size**: Set the width and height of the animation area.
  * **Max Fireworks**: Controls how many fireworks can be on screen at once.
  * **Time Scale**: Slow down the animation for a slow-motion effect.
  * **Blur Control**: Adjusts the amount of soft, glowing particles in explosions. Set to `0` for only sharp sparks.
  * **Enable Stereo 3D**: Toggles the side-by-side 3D view.
  * **Start/Stop Recording**: Captures the animation and downloads it as a video file.

-----

## How to Use Custom Fonts

To display the message in a different language:

1.  **Get a Font**: Download a font file (`.ttf` or `.otf`) that supports your language (e.g., from [Google Noto Fonts](https://fonts.google.com/noto)).
2.  **Convert the Font**:
      * Go to the online **[Facetype.js](https://www.google.com/search?q=https://gero.github.io/facetype.js/)** converter.
      * Upload your font file.
      * **Important**: Paste all the unique characters you want to use into the text box.
      * Convert and download the resulting `.json` file.
3.  **Use the File**:
      * Rename the downloaded file to exactly **`FavLang.json`**.
      * Place it in the same folder as your project's HTML file.
      * Run the application and check the "Use Custom Font" box.

-----

## Technology Stack

  * HTML5
  * CSS3
  * JavaScript (ES6 Modules)
  * **Three.js** for 3D rendering and effects.
