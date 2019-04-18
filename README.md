<h2 align="center"><a href="https://www.ls.haw-hamburg.de/~SIMLab/"><img src="assets/img/ESIcon.svg" title="ESIcon" width="250" alt="ESIcon"></a><br>Emergency Simulator</h2>
<p align="center"><strong>WebApp for Emergency Training Situations</strong></p>

| TraineeView | TrainerView |
| -| - |
| ![TraineeView GIF](https://media.giphy.com/media/Zy7tAf9dW352WuzmEc/giphy.gif) | ![TrainerView GIF](https://media.giphy.com/media/1ZDDxmQpVG8nA4I6zU/giphy.gif) |

---

## Want to use the App?
You are interested in learning about this product without wrapping your head around the sourcecode? - Head over to our [Wiki-Page](https://github.com/SIMLabHAW/SIMLab-Emergency-Simulator/wiki), where we tell you all about the project background, its features and how to install the Emergency Simulator in all detail. 

If terms like *IP address*, *localhost* or *XAMPP* sound familiar, continue with the installation process here.

---

## Quick Installation Guide

- To use the Emergency Simulator, a device functioning as server and local area connection between devices is required. One possibility to build up such an environment is e.g. to use <a href="https://www.apachefriends.org/de/index.html" target="_blank">XAMPP</a> in combination with a wlan hotspot.
- When the codebase is downloaded, the initial name of the archive is ```SIMLab-Emergency-Simulator-master.zip```. It is *highly* recommended to rename the unzipped folder to **esim**.
- When using XAMPP, the previously downloaded folder (now named **esim**) needs to be placed in *htdocs*. (*htdocs* is a subfolder in the XAMPP installation directly, e.g. ```C:/xampp```
  - If another name e.g. *my_name* is chosen as foldername instead of *esim*, the app can be accessed using the ```server_ip_adress/my_name/```. 
- A *modern* internet browser is required to run the application.
  - If the browser is to old to run the app, a popup will notify the user at ```login.html```.

---

## Team

Developers:
- <a href="https://github.com/GitHelge" target="_blank">**Christian Bauer**</a>
- <a href="https://github.com/HappyLychee" target="_blank">**Serena Glass**</a>
- Christine Geßner
- Chahinez Chaouchi

Wiki Contributors:
- Alexandre H. Mendes
- Katrin Rowe

Project Lead:
- <a href="https://www.ls.haw-hamburg.de/~SIMLab/index.php/kontakt.html" target="_blank">`Prof. Dr. Boris Tolg`</a>
- <a href="https://www.ls.haw-hamburg.de/~SIMLab/index.php/kontakt.html" target="_blank">`Prof. Dr. Stefan Oppermann`</a>

---

## FAQ

- **Why are all the dependencies included in the project?**
    - The Emergency Simulator was ment be able to work without a stable internet connection. 
    Therefore, with e.g. the use of a low cost wifi-hotspot, trainings with two connected devices
    can be perfomed.
- **How to find out the IP adress of my server?**
    - The method to find the current IP adress is depending on the operating system of the server. 
      - If windows is used, the IP Adress can be found using the *command line* and issuing the command *ipconfig*. Then look for the entry: *IP Adress*.
      - For macOS, use the *Terminal* and type *ifconfig | grep "inet "*. 
      - For other operating systems, refer to external sources.

---

## Code Documentation
Code Documentation can be found [**here**](https://githelge.github.io/es_doc/). 

---

## Contributions

In this section, a lot of potential improvements are hinted at. If you want to contribute to this repository and project, feel free to fork or clone.

### Potential Changes and Features for Future Versions

Many of the already implemented features are listed on a <a href="https://docs.google.com/spreadsheets/d/1kEWTkjUGEv1Msgwj1EuNwlg2URnYAXst4ZItrPl_gXs/edit?usp=sharing" target="_blank"> GoogleSpreadsheet</a>. However, there are more general ideas to further improve the Usability, Application and Codebase: 

#### Usability
- Create an *easy to navigate* website containing the wiki, pictures and other media.
- Evaluate the possibility of creating an installer for improved usability. 
- Create a localized (e.g. german) version.

#### Application Features
- Implement a *storyboard* for preconfiguring szenario paths.
- Simulate baseline drift instead of flat curves.
- Implement the calculation and visualization of a 12-channel ECG.
- Improve *in-training*-documentation of parameter changes and trainee reactions.
- Generate statistical evaluaiton of the trainee reactivity.
- Improve the PDF export feature in general. 
- Evaluate if multiple user-accounts are necessary.

#### Code Adaptions
- Perform code quality improvements (e.g. ESLint)
- Implement all "TODO"'s which are marked throughout the code.
- Save screenshots in the database instead of the folder structure on the server.
- Improve HTML parts in terms of:
  - Extended Comments for readability;
  - (More) CSS classes instead of styles.
- Move from myQSL to e.g. ReThinkDB, as most persistently saved stuff is already saved as json strings.
- Use Node.js as Backend-Solution instead of PHP.
- Go for TypeScript as alternative to JS for syntactic sugar. 

---

## Credits

Following projects were used in this work:
- Bootstrap v4.0.0 <a href="https://getbootstrap.com" target="_blank">`getbootstrap.com`</a>
- JQuery v3.2.1 <a href="http://jquery.com" target="_blank">`jquery.com`</a>
- Popper <a href="https://popper.js.org" target="_blank">`popper.js.org`</a>
- html2canvas v1.0.0-alpha.12 <a href="https://html2canvas.hertzen.com" target="_blank">`html2canvas.hertzen.com`</a>
- Ion.RangeSlider v2.2.0 <a href="https://github.com/IonDen/ion.rangeSlider" target="_blank">`github.com/IonDen/ion.rangeSlider`</a>
- FPDF v1.81 <a href="http://www.fpdf.org" target="_blank">`fpdf.org`</a>
- Font Awesome Free v5.4.1 <a href="https://fontawesome.com" target="_blank">`fontawesome.com`</a>
- Natural Docs v2.0 <a href="https://www.naturaldocs.org" target="_blank">`naturaldocs.org`</a>
- ...further sources are named in each file.

## License
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

- **[GPL v3 license](https://www.gnu.org/licenses/gpl-3.0)**
- Copyright (C) 2018 <a href="https://www.ls.haw-hamburg.de/~SIMLab/" target="_blank">HAW-Hamburg</a>.
