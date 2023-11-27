---
title: Installing SplashKit SDK on WSL
description: A guide on installing SplashKit SDK on WSL.
---

Once installed, launch the WSL distribution you installed. This will open a terminal window running a Linux environment.

1. Update the package lists and upgrade the installed packages by running the following commands in the Linux terminal: Run the following at the Terminal:

    ```bash
    sudo apt update
    ```
    ```bash
    sudo apt upgrade
    ```
  

1. Install the necessary dependencies for SplashKit by running the following command:

    ```bash
    sudo apt install git curl
    ```
    ![](https://i.imgur.com/ZKXjGyV.png)

    ***OPTIONAL*** Install the required dependencies: SplashKit requires several dependencies to be installed. Run the following command in the WSL terminal to install them
    ```bash
    sudo apt install build-essential libsdl2-dev libsdl2-image-dev libsdl2-ttf-dev libsdl2-mixer-dev
    ```

    
1. Download and install SplashKit using the SKM (SplashKit Manager) installation script. Run the following command in the Linux terminal:
    `bash <(curl -s https://raw.githubusercontent.com/splashkit/skm/master/install-scripts/skm-install.sh)`

    This can also be found on the [SplashKit](http://www.splashkit.io) home page.
1. Check if the skm executable is present in the .splashkit directory by running the following command:
    ```bash
    ls -l .splashkit
    ```
    ![Screenshot](https://i.imgur.com/Rj6RtnH.png)
    This will list the contents of the .splashkit directory, including the skm executable.
1. If the skm executable is present, you can add it to your system's PATH by running the following command:
    ```bash
    echo 'export PATH="$HOME/.splashkit:$PATH"' >> ~/.bashrc
   source ~/.bashrc
   ```
   ![](https://i.imgur.com/s0XAzJw.png)
   ***OPTIONAL*** Install SKM tools for Linux:
   `skm linux install`
   ![](https://i.imgur.com/JtAFvq5.png)

1. Execute `skm` to test it was successfully installed.

    ```bash
    skm
    ```

    You should see the following messages:

    ```bash
    SplashKit is installed successfully!
    Missing skm command. For help use 'skm help'
    ```

    SplashKit supports a number of languages. Run `skm help` at the terminal to see the different commands you can run.

