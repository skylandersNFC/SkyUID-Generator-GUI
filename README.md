----------------------------------------

# SkyUID Generator GUI

*Disclaimer: **This script won't work for Imaginators dumps, only from SSA to SSC.**

----------------------------------------
**What is this:**

This is a python GUI app that can create Skylander dumps, adjusted for a specific card UID.

It's helpful if you have NFC UID locked cards (Sector 0, Block 0 Read-Only) and you need to prepare each dump before flashing it, so it's aligned with the UID of your card.

----------------------------------------

**How to run it:**

1. **SkyUID-Generator-GUI** now has an **EXE compiled** version with **PyInstaller**, which means you **don't need Python installed to run it**.

2. Download the **Windows** version for "**![Releases](https://github.com/skylandersNFC/SkyUID-Generator-GUI/releases/)**" (SkyUID-Generator-GUI-Windows.zip)

3. Extract it somewhere and run the "**SkyUID-Generator-GUI-WIN.exe**"
![SkyUID-Generator-GUI-Windows.exe](https://i.ibb.co/m5z5dXn/image.png)

4. Now you should have the **GUI** running. It will look something like this
![01. SkyUID-Generator-GUI](https://raw.githubusercontent.com/t3hsuppli3r/SkyUID-Generator-GUI/main/img/01.%20SkyUID-Generator-GUI.jpg)

5. On the first "**UID**" field, you only need to provide your card **UID** in order for the script to generate a proper Skylander dump for it.
![03. Dump Selected](https://raw.githubusercontent.com/t3hsuppli3r/SkyUID-Generator-GUI/main/img/03.%20Dump%20Selected.jpg)

6. You can get a **UID** of a card by just placing it on the reader and pressing "**READ TAG**". That's the first thing it will tell you. The **UID** in this example is different from the **UID** in the field, but that's just an example. Also **remove any spaces** from the UID so it's "**EF844A3E**" (example)
![00. How to get UID with MWT](https://github.com/skylandersNFC/SkyUID-Generator-GUI/blob/main/img/00.%20How%20to%20get%20UID%20with%20MWT.jpg)

7. On the second field you need to **pick a Skylander from the dropdown menu**. The skylanders listed in the dropdown are from the "[Skylanders Ultimate NFC Pack](https://docs.google.com/document/d/1M3CXm2UcXLo1kuhYmAAtitfPJUJoyL47Ey95BYIt-Z0/edit?usp=sharing)". Since they are sorted into folders, you **need to go deep enough** until you have **selected a single Skylander** dump and see a result in the "**Output File**" field.
![02. UID and Dumps Dropdown](https://raw.githubusercontent.com/t3hsuppli3r/SkyUID-Generator-GUI/main/img/02.%20UID%20and%20Dumps%20Dropdown.jpg)

8. After **generating a UID** specific dump file, you should see this 
![04. Generating Dump with Specific UID](https://raw.githubusercontent.com/t3hsuppli3r/SkyUID-Generator-GUI/main/img/04.%20Generating%20Dump%20with%20Specific%20UID.jpg)

9. **Check the main directory**. There you should see your **new dump file**. For example "**UID_24A3C48A_Boomer.dump**"

10. That's it. This new dump file will be **adjusted** for the **specific UID** that you have provided. Now **flash** it onto **your card** with MWT or whatever tool you are using. You **will get 63 out of 64** blocks written, and that's **perfectly fine**. The whole idea of SkyUID is that **we don't touch Sector 0, Block 0** on the card (since it's Read-Only), but we **adjust the rest of the data** in the dump file so it can be synchronized with the already existing **Sector 0, Block 0 (UID block)** on the card.
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
