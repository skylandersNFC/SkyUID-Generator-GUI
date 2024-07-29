----------------------------------------

# SkyUID Generator GUI

*Disclaimer: **This script won't work for Imaginators dumps, only from SSA to SSC.**

----------------------------------------
**What is this:**

This is a python GUI app that can create Skylander dumps, adjusted for a specific card UID.

It's helpful if you have NFC UID locked cards (Sector 0, Block 0 Read-Only) and you need to prepare each dump before flashing it, so it's aligned with the UID of your card.

----------------------------------------

**How to run it:**

1. Install Python from here: https://www.python.org/downloads/. Get the latest version.

2. Back to GitHub - Click on the green "**<> Code**" button on the upper right and then "**Download ZIP**".
Additionally, you can also go to "**Releases**" on the right side of the screen and then download the "**SkyUID-Generator-GUI-1.0.zip**".
It's the same thing.

3. Extract the archive somewhere, let's say "**D:\Downloads\SkyUID-Generator-GUI-main**" (for example)
   
4. If you have a proper Python .py file extension associated, you can run it by just double clicking on the "**main.py**" file.
  
5. If not, run it via `python main.py` command inside **CMD** from the same directory where the script is. In our case this should be "**D:\Downloads\SkyUID-Generator-GUI-main**"

6. If you don't know how to use **CMD**, google it or ask ChatGPT.

7. Now you should already have the python GUI running. It will look something like that
![01. SkyUID-Generator-GUI](https://raw.githubusercontent.com/t3hsuppli3r/SkyUID-Generator-GUI/main/img/01.%20SkyUID-Generator-GUI.jpg)

8. On the first "UID" field, you only need to provide your card UID in order for the script to generate a proper Skylander dump for it.
![03. Dump Selected](https://raw.githubusercontent.com/t3hsuppli3r/SkyUID-Generator-GUI/main/img/03.%20Dump%20Selected.jpg)

9. You can get a UID of a card by just placing it on the reader and pressing "READ TAG". That's the first thing it will tell you. The UID in this example is different from the UID in the field, but that's just an example. Also remove any spaces from the UID so its "EF844A3E" (example)
![00. How to get UID with MWT](https://github.com/skylandersNFC/SkyUID-Generator-GUI/blob/main/img/00.%20How%20to%20get%20UID%20with%20MWT.jpg)

10. On the second field you need to pick a Skylander from the dropdown menu. The skylanders listed in the dropdown are from the "[Skylanders Ultimate NFC Pack](https://docs.google.com/document/d/1M3CXm2UcXLo1kuhYmAAtitfPJUJoyL47Ey95BYIt-Z0/edit?usp=sharing)" (V5), so pretty much the best dumps out there you can find.
![02. UID and Dumps Dropdown](https://raw.githubusercontent.com/t3hsuppli3r/SkyUID-Generator-GUI/main/img/02.%20UID%20and%20Dumps%20Dropdown.jpg)

11. The dump files are sorted with folders so you need to go inside them using the dropdown menu in order to select the dumps. If you made a mistake, just click on "<<Back"

12. After generating a UID specific dump file, you should see this 
![04. Generating Dump with Specific UID](https://raw.githubusercontent.com/t3hsuppli3r/SkyUID-Generator-GUI/main/img/04.%20Generating%20Dump%20with%20Specific%20UID.jpg)

13. Check you script main directory. In our example that's "**D:\Downloads\SkyUID-Generator-GUI-main**". There you should see your new dump file. For example, "**UID_24A3C48A_Boomer.dump**"

14. That's it. This new dump file will be adjusted for the specific UID that you have provided it. Now flash it onto your card with MWT or whatever you are using.
----------------------------------------

### Special thanks to:

>[A crushing individual from Discord]() - who refactored the code, added GUI and everything.
>
>[DevZillion](https://github.com/DevZillion) - [TheSkyLib](https://github.com/DevZillion/TheSkyLib)
>
>[Vitorio Miliano]() - [libs/tnp3xxx.py](https://github.com/DevZillion/TheSkyLib/blob/main/libs/tnp3xxx.py)
>
>[Toni Cunyat](https://github.com/elbuit) - [libs/sklykeys.py](https://github.com/DevZillion/TheSkyLib/blob/main/libs/sklykeys.py)
>
>[Nitrus](https://github.com/Nitrus) - [libs/UID.py](https://github.com/DevZillion/TheSkyLib/blob/main/libs/UID.py)

----------------------------------------
