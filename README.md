
<p align="center">

  <img src="https://github.com/Motobug/Badnik-Stream-Tool/blob/master/Preview.png" alt="Preview">
  
</p>

<h1 align="center">Badnik Stream Tool</h1>

This is a stream tool based on [Readek's](https://github.com/Readek/RoA-Stream-Tool) and [ilikepizza's](https://github.com/ilikepizza107/Project-Plus-Stream-Tool), with a focus on readability, 4:3, and attractive design. 
---

## Features
- [Easy and fast setup](https://file.garden/Zf2bnkmk1CN8FNMM/Setup.mp4) using a browser source. Drag and drop!
- [Handy interface](https://file.garden/Zf2bnkmk1CN8FNMM/GUIDemo.mp4) to quickly change everything you need, like player names, pronouns, characters, scores, round, casters...
  - With customizable **Player and Commentator Presets** to setup your match in no time!
- Every single character and skin the game has to offer is supported (more than 600 different skins!).
- A [16:9](https://raw.githubusercontent.com/ilikepizza107/Project-Plus-Stream-Tool/master/Git%20Images/16-9.png) and [4:3](https://raw.githubusercontent.com/ilikepizza107/Project-Plus-Stream-Tool/master/Git%20Images/4-3.png) overlay!
- A "[VS Screen](https://file.garden/Zf2bnkmk1CN8FNMM/VSDemo.mp4)" to be displayed when waiting for the next game.
- A [Bracket View](https://raw.githubusercontent.com/ilikepizza107/Project-Plus-Stream-Tool/master/Git%20Images/BracketPreview.png) to showcase your tournament's top 8 positions!
- A [Remote GUI](https://raw.githubusercontent.com/ilikepizza107/Project-Plus-Stream-Tool/master/Git%20Images/RemoteGUI.png) that can be accessed by any device within the local network, including mobile devices!
- Now with [2v2 support](https://raw.githubusercontent.com/ilikepizza107/Project-Plus-Stream-Tool/master/Git%20Images/2v2.png)!

---

## How to setup
These are instructions for **OBS Studio**:
- Get the [latest release](https://github.com/ilikepizza107/Project-Plus-Stream-Tool/releases).
- Extract somewhere.
- Drag and drop `4.3 Scoreboard.html` into OBS, or add a new browser source in OBS pointing at the local file.
  - If the source looks weird, manually set the source's properties to 1920 width and 1080 height, or set your OBS canvas resolution to 1080p, or make the source fit the screen (Ctrl+F).
- In the source's properties, change *Use custom frame rate* -> `60` (if streaming at 60fps of course).
- Manage it all with the `Project+ Stream Tool` executable (or project-st-gui.app if you are on Mac).

Repeat from the 3rd step to add the `VS Screen.html` and `Bracket.html` views, though I recommend you to do so on another scene.

### Interface shortcuts!
- Press `Enter` to update*.
- Press either `F1` or `F2` to increase P1's or P2's score.
- Press `ESC` to clear player info*.

***Functionality may change in some menus to ease workflow.**

For developing, there are some shortcuts to make things easier:
- Press `F5` to reload the GUI.
- Press `F12` to open the dev console. This will also unlock window resolution.

---

## Advanced setup
Yes, those instructions above are enough, but we can do better. **All of this is optional** of course.
 
2 basic transitions are included in the `Resources/OBS Transitions` folder, intended to be used to change to the game scene and to the VS screen, if you don't have a transition yourself of course. To use them on OBS:
- Add a new stinger transition.
- Set the video file to `Game In.webm` if creating the game scene transition, and `Swoosh.webm` if creating a VS screen transition.
- Transition point -> `350 ms`.
- I recommend you to set the Audio Fade Style to crossfade, just in case.
- On the scene's right click menu, set it to Transition Override to the transition you just created.
- Also, you may want to set a hotkey to transition to the game scene so you can press enter ingame to start the replay and press the transition key at the same time. The transition is timed to do so.

### Remote GUI

The Stream Tool GUI can be controlled remotely by any device within the local network where the GUI is running, and yes, this includes mobile devices! Please take a look at Readek's [wiki](https://github.com/Readek/RoA-Stream-Tool/wiki/8.-Remote-GUI) for instructions.

---

## Other stuff...
Do you want to customize something? Do you need some OBS tips and tricks for a Project+ stream? **Please, go to Readek's [wiki](https://github.com/Readek/RoA-Stream-Control/wiki)**!
