# Wunduniik V6 on Linux: A User's Guide 🐧

Wunduniik V6 is not officially supported on Linux by the modlist's creator, Alaxouche. However, with a few extra steps, the Wabbajack installation can be adapted to work successfully. This guide assumes you have a basic understanding of Linux and Mod Organizer 2 (MO2).

### 1. The Omni-Guide's Automation Script

The recommended method for installing Wunduniik V6 on Linux is to use the **Omni-guides.sh** script. This script handles many of the complexities of getting Wabbajack and MO2 running on a Linux system.

* Follow the instructions provided in the [Omni-guides Wabbajack Modlist Linux Wiki](https://github.com/Omni-guides/Wabbajack-Modlist-Linux/wiki/Using-the-omni%E2%80%90guides.sh-Automation-Script) to install the modlist.

> **Note:** When you launch Mod Organizer 2 for the first time, you will likely see an error message related to Frame Generation. You can safely click **OK** and proceed with the rest of the guide. This issue will be resolved in a later step.

### 2. Configure Mod Organizer 2

Once the Omni-guides script has successfully completed its installation, you need to make a few specific changes inside Mod Organizer 2 (MO2) to properly launch Wunduniik.

* In MO2, locate the executable dropdown menu (it's usually in the top right corner).
* Change the selected launcher from the default to **Wunduniik Legacy**.

### 3. Fixing the Frame Generation Error

To resolve the Frame Generation error, you must manually delete a specific flag file.

* Navigate to your MO2 plugins directory. The path will vary depending on your setup, but it's typically within the main Wabbajack installation folder.
* Inside the plugins folder, find the `FrameGenCompatibilityCheck` folder.
* Within that folder, **delete the file named `firstrun.flag`**.
* After deleting the file, restart Mod Organizer 2.

### 4. Troubleshooting

#### Game Closes Immediately After Launch

If the game immediately closes after a brief loading screen (specifically after showing the `VFS` logs), you may need to force the vanilla launcher to generate a configuration file.

* In MO2, open the executable dropdown menu and select **Edit**.
* Click the **+** button at the top of the list to add a new executable.
* Select **Add from file...**
* Navigate to your modpack's installation folder, then open the `Game Root` folder.
* Select `SkyrimSELauncher.exe` and click **Open**.
* Press **OK** to save the new executable.
* Now, select the newly added **SkyrimSELauncher** from the executable dropdown and click **Run**.
* The vanilla launcher will open and automatically select a graphics preset for you. You do not need to change anything.
* **Close the vanilla launcher window** and change the MO2 executable back to **Wunduniik Legacy**.

### 5. Enjoy Wunduniik V6 on Linux! 🎉

You should now be able to launch Wunduniik V6 and play it on your Linux machine. If you encounter any further issues, please refer to the **Wabbajack Discord server in the #unofficial-linux-help channel** for troubleshooting assistance.
