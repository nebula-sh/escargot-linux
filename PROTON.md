# escargot-linux (Proton)

This is a tutorial on how to install Windows Live Messenger (escargot [escargot.chat) on Linux.

First, download WLM 7.5 from the Escargot website
OR
wget it
`https://storage.levelleap.com/nina/clients/msnp/patched-installer/msn/escargot-msn-7.5.0324-en.zip`

Now that you have it downloaded, unzip it
You need: steam, flatpak, protontricks

Arch-Based
`sudo pacman -S steam flatpak`
Ubuntu-Based (You might need to add the flatpak repo)
`sudo apt install steam flatpak`

Now that you have to get these two programs

Install protontriclks
`flatpak install flathub com.github.Matoking.protontricks`

Then, open steam and add the WLM exe
`+ Add a game > Add a Non-Steam Game > Browse (select WLM exe) > Add selected programs`

Then, boot up protontricks
`flatpak run com.github.Matoking.protontricks`

Select your WLM file name (if you didn't change it), then select the default wine prefix

Now click
`Install a Windows DLL library or component`

Search up vb on your keyboard
`Select vb2run, vb3run, vb4run, vb6run`
and install the Visual Basic libs

Then boot up the WLM installer (through Steam)
Install it as you normally would

Then go into the properties of the added program on Steam
Change the `Target` path to your `RUN_AFTER_INSTALL.exe` file

After you do that, boot up the program (through Steam)
Patch as you normally would

Now, go back to the program properties
Look at the directory in top of the protontricks bar (the bar where there is the close button)
Copy it and paste it into the `Target` path like you did with the `RUN_AFTER_INSTALL.exe` file

Now that you copy and pasted it, add quotations at the front and end of the path, add the following to the end of the path
`Program Files (x86)/MSN Messenger/msnmsgr.exe`

Your `Target` path should look something like this
`"home/micheal/.local/share/Steam/steamapps/compatdata/3359716659/pfx/drive_c/Program Files (x86)/MSN Messenger/msnmsgr.exe"`

Now, this should be all, boot up the program on Steam and it should work! Thanks for reading, for Wine, go to the WINE.md file.

Micheal 2024
