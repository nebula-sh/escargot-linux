# escargot-linux

This is a tutorial on how to install Windows Live Messenger (escargot [escargot.chat) on Linux.

First, download WLM 7.5 from the Escargot website
OR
wget it
`https://storage.levelleap.com/nina/clients/msnp/patched-installer/msn/escargot-msn-7.5.0324-en.zip`

Now that you have it downloaded, unzip it
You need: wine, winetricks

Arch-Based
`sudo pacman -S wine winetricks`
Ubuntu-Based (this might require the keyrings and the repo from the wine website)
`sudo apt install wine winetricks`

Now that you have to get these two programs

Install Visual Basics 2-6 (not including VB5)
`winetricks vb2run vb3run vb4run vb6run`

First, install Windows Live Messenger
`wine escargot-msn-7.5.0324-en.msi`

After you've done that, run the run after install exe
`wine RUN_AFTER_INSTALL.exe`
Patch like you normally would

Now, this should be all! Thanks for reading, for Proton, go to the PROTON.md file.

Micheal 2024
