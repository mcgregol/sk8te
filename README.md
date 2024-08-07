# SK8TE User Manual by ACHIEVE

SK8TE is your tool to configure and manage Stryd sensors. Capabilities include player assignment, clock synchronization, hardware identification, and data extraction.

## Installation

Currently, SK8TE is compatible with **Windows 10/11 PCs** with Bluetooth capabilities. You can download the latest installer [here](https://github.com/mcgregol/sk8te/releases). Once downloaded, run the installer.

![1](https://github.com/mcgregol/sk8te/blob/main/thumbnail.png?raw=true)

> **Note:** if you receive a "Windows protected your PC" message, select **More info**, then **Run anyway**. The SK8TE application was not designed by Microsoft, hence the warning. 

You may now proceed through the installation.

## Basic Usage

Once installed, SK8TE can be accessed through the **Start Menu** or via **desktop shortcut** if opted into by the user during installation. Below is the main screen of the application.

![main](https://github.com/mcgregol/sk8te/blob/main/main.png?raw=true)
In order to begin interacting with the Stryds, we need to scan for available ones. Please ensure any Stryds you intend on working with are sufficiently charged and within close proximity to your computer.
> **Note:** Please ensure bluetooth is enabled

To begin, select **Scan**<sup>[1]</sup> to begin a 10 second scan for available devices. Once the scan is completed, a list of hardware addresses will appear in the **sensor listbox**<sup>[2]</sup>.

### Blink

All your files and folders are presented as a tree in the file explorer. You can switch from one to another by clicking a file in the tree.

### Erase

You can rename the current file by clicking the file name in the navigation bar or by clicking the **Rename** button in the file explorer.

### Sync Clock

You can delete the current file by clicking the **Remove** button in the file explorer. The file will be moved into the **Trash** folder and automatically deleted after 7 days of inactivity.

## Assign Devices and Build Your Team

You can export the current file by clicking **Export to disk** in the menu. You can choose to export the file as plain Markdown, as HTML using a Handlebars template or as a PDF.

### Importing and Exporting a Team

## Exporting Data

Synchronization is one of the biggest features of StackEdit. It enables you to synchronize any file in your workspace with other files stored in your **Google Drive**, your **Dropbox** and your **GitHub** accounts. This allows you to keep writing on other devices, collaborate with people you share the file with, integrate easily into your workflow... The synchronization mechanism takes place every minute in the background, downloading, merging, and uploading file modifications.

There are two types of synchronization and they can complement each other:

- The workspace synchronization will sync all your files, folders and settings automatically. This will allow you to fetch your workspace on any other device.
	> To start syncing your workspace, just sign in with Google in the menu.

- The file synchronization will keep one file of the workspace synced with one or multiple files in **Google Drive**, **Dropbox** or **GitHub**.
	> Before starting to sync files, you must link an account in the **Synchronize** sub-menu.
