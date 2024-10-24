# SK8TE User Manual by ACHIEVE

SK8TE is your tool to configure and manage SK8TE sensors. Capabilities include player assignment, clock synchronization, hardware identification, and data extraction; all within a team setting on one or multiple sensors.

## Installation

Currently, SK8TE is compatible with **Windows 10/11** machines with Bluetooth capabilities. You can download the latest installer [here](https://github.com/mcgregol/sk8te/releases/latest). Once downloaded, run the installer.

![1](https://github.com/mcgregol/sk8te/blob/main/thumbnail.png?raw=true)

> **Note:** if you receive a "Windows protected your PC" message, select **More info**, then **Run anyway**. The SK8TE application was not designed by Microsoft, hence the warning. 

You may now proceed through the installation.

## Basic Usage

Once installed, SK8TE can be accessed through the **Start Menu** or via **desktop shortcut** if opted into by the user during installation. Below is the main screen of the application.

![main](https://github.com/mcgregol/sk8te/blob/main/main.png?raw=true)

In order to begin interacting with the sensors, we need to scan for available ones. Please ensure any sensors you intend on working with are sufficiently charged and within close proximity of your computer.
> **Note:** Please ensure bluetooth is enabled

To begin, select **Scan**<sup>[1]</sup> to begin a 10 second scan for available devices. Once the scan is completed, a list of hardware addresses will appear in the **sensor listbox**<sup>[2]</sup>. You may select or deselect any number of devices by individually **clicking** them or **dragging** over them. **All** selected sensors will be queued when the user executes the following actions:

### Blink

Sensor(s) will asynchronously flash their LED until stopped by the user. The blink function is useful for identifying and tracking physical sensors within the application.
>**Example:** A specific sensor in the SK8TE app needs to be physically labelled

### Erase

Sensor(s) onboard storage will be cleared. This cannot be undone and any data not exported will be **lost** permanently. It is advisable to routinely erase sensors in order to reduce unnecessary data export time.

### Sync Clock

Sensor(s) internal clock will be synchronized with the clock of the computer running the SK8TE app. The timestamps within data collected by a SK8TE sensor will **not** be correct if the sensor clock is out of sync.
>**Note:** If the computer clock is wrong during synchronization, the sensors's clock will also be wrong

## Assign Devices and Build Your Team

In order to collect accurate data and increase ease of use, it is important to assign a player to a device. You can update player attributes such as weight, player name/number, etc. Once assigned, the SK8TE app will list the player's information in the listbox. Unassigned players will be displayed using their MAC address. In the diagram below, the first sensor<sup>[4]</sup> **has** been assigned, whereas the second sensor<sup>[5]</sup> **has not.**

![diag](https://github.com/mcgregol/sk8te/blob/main/Screenshot%202024-08-07%20123129.png?raw=true)

To begin, select as many sensors as you need players assigned from the listbox. Next, select the **(Re)assign**<sup>[3]</sup> button from the interface. A new form will be opened.
>**Note:** Both unassigned and assigned sensors can be selected simultaneously.

![fdf](https://github.com/mcgregol/sk8te/blob/main/form.png?raw=true)

The sensor label<sup>[6]</sup> displays the current sensor being assigned. In this case, the sensor was already assigned, so the existing player name is displayed next to the hardware address, and the current number and weight are in their respective input boxes. The user then inputs the player name, number, and weight. While this process is taking place, this sensor will **blink** indefinitely, stopping only when **Skip**<sup>[8]</sup> or **Next**<sup>[9]</sup> is selected and changes are made to the device.
>**Note:** It is recommended to physically label a sensor while it is blinking during assignment.

As you can see in the top right of the form<sup>[7]</sup>, this sensor is the first of two selected for assignment. Once this sensor is assigned or skipped, the program will move to the next one, which will begin blinking, and the assignment process will repeat until all sensors in the list are iterated through.

### Importing and Exporting a Team
Although an assigned sensor's weight is persistently saved to the hardware of the sensor, player assignments are stored on the computer running the SK8TE app. As a result, these assignments only originally register to that instance of SK8TE.
>**Note:** Be sure to export your team assignments before upgrading SK8TE, as they **will** be overwritten.

To export SK8TE sensor player assignments, navigate to the top left of the screen and select **Extra** > **Export Database**. Specify a filename (such as the team name),  and save the JSON file. These player assignments can now be used on another device running SK8TE. To import, select **Extra** > **Import Database**.

## Exporting Data

On the far right of the screen is the export data section, displayed in the figure below. Data retrieved from a sensor is saved to the computer running SK8TE. To specify the location of this this data once saved, select **Update Save Path**<sup>[10]</sup>. The current save path<sup>[11]</sup> will reflect these changes.

![export](https://github.com/mcgregol/sk8te/blob/main/export.png?raw=true)

To begin the export, select desired sensors from the listbox, and then **Export Data**<sup>[12]</sup>. Data transfer between the sensors and computer will begin, with the **total** progress displayed in the bar<sup>[13]</sup>. Also displayed, will be the current sensor that is exporting.
