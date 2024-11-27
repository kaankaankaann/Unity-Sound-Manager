# Unity Sound Manager

A simple and extensible sound management system for Unity, designed to handle audio playback, sound toggling, and sound editing through ScriptableObjects.

## Features

- **Centralized Sound Management**: Play sounds and control the global audio state from a single point using `SoundManager`.
- **ScriptableObject Sound Data**: Use a `SoundSO` to define and store sound settings (name, audio clip, volume, pitch).
- **Custom Inspector**: The `SoundSOEditor` provides a custom editor for easily managing sound properties and previewing sounds directly within Unity's inspector.
- **Sound Data Persistence**: Sound settings are saved and loaded automatically using `PlayerPrefs`, allowing users to retain sound preferences across sessions.
- **Editor Menu**: Quick access to create and manage sound data through an editor menu.
- **Mute/Unmute**: Toggle sound on or off globally.

## Getting Started

### 1. Install and Setup
- Download the [SoundManager](#../SoundManager.unitypackage).
- Open the downloaded `.unitypackage` file and import all the assets.
- After importing, you should see the necessary scripts and resources in your `Assets` folder.

### 2. Adding Sounds
- Open the newly created `SoundData` asset from the Editor Menu by selecting `Databases -> Open Sound Database` in the Unity editor.
- Add sounds using the custom inspector. You can define the name, clip, volume, and pitch for each sound.

### 3. Using the Sound Manager
- Call `SoundManager.Initialize()` to initialize sound management.
- To play a sound, use `SoundManager.Play("SoundName")`.
- You can toggle sound on/off globally by calling `SoundManager.ToggleSound(true)` or `SoundManager.ToggleSound(false)`.
