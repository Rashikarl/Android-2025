# Android-2025
Full Android Info 

logo


The AndroidIDE Wiki
Guide, tips and tricks and general information about AndroidIDE.

Introduction
AndroidIDE is an Integrated Development Environment (IDE) to build Gradle based Android projects on Android devices.

Installation
  Installation guide.

Minimum requirements
Setup the terminal
Build Tools Installation
Getting started
  Getting started guide for newbies.

Creating a new project
Working with an existing project
Working with projects
  Get familiar with the various elements of the editor screen.

Options menu.
File tree.
Bottom sheet.
Code editor.
UI Designer.
Important links
The AndroidIDE Website
For latest updates, join the Telegram Channel
For discussions, join the Telegram group
Source code for all AndroidIDE projects can be found in the AndroidIDE GitHub Organization.

LOVE WHAT YOU SEE?
logo
AndroidIDE.
© 2021-2023 AndroidIDE

SOCIALS
Installation
Getting Started
UI Designer

Editor
AndroidIDE
Installation
This guide shows how to install AndroidIDE, setting up the terminal and the Android build tools installation.

Before getting started, please make sure that your Android device meets the minimum requirements.

Minimum requirements
ARM based CPU arm64-v8a (a.k.a aarch64) or armeabi-v7a.
At least 1.5GB of RAM available for use (not total RAM).
At least 4GB of free space is recommended. Around 1.5GB for installation and rest for other dependencies that you might need to download depending on your project.
Setup the terminal
Open AndroidIDE terminal. It will install the bootstrap packages.
Then run pkg upgrade to update packages to latest version.
Build Tools Installation
Install the JDK, SDK and commandline tools for sdk.

Open terminal and run idesetup -c.
After you execute the above command, it'll show a summary of the configuration. Type y to confirm the configuration and start the installation process.
After successful installation, Downloads completed. You are ready to go! will be printed.
You can execute idesetup -h to see configuration options.

Footnotes
Cheatsheet :

One command to setup the terminal and to install build tools.
cd && pkg upg && idesetup -c
↩ ↩

logo


Getting Started
This guide shows how to get started with AndroidIDE and build an Android application. Before proceeding, please make sure that you have installed the build tools. If not, see the installation guide.

Creating a new project
Creating a new project is simple. Simply open AndroidIDE and click on the Create project button.

There are project templates available which setup some basic things for you. You can choose a template of your choice.

After you select the project template, you'll be asked to enter the details about your application. Enter the application name and it's package name. You could also choose the directory where the project will be created along with the application's minimum and target SDK.

Once you're done with above things, click the 'Create project' button.

Working with an existing project
To open an existing project in AndroidIDE, click the Open existing project in the main activity. This opens the SAF file picker where you can choose the project directory you want to open.

Gradle based Android projects are supported. However, it is currently not possible to build projects that use older versions of the Android Gradle Plugin. To be able to build a project in AndroidIDE, your project must use Android Gradle Plugin v7.2.0 or newer.

For people trying to build projects developed with other older IDEs, you might need to update your build scripts before opening the project in AndroidIDE.

More info
Once you create a new project or open an existing project, the IDE will open the editor and will start to sync the project. If this is the first time you're building a project on AndroidIDE, it might take a while to set things up. It totally depends on your internet connection. To see the build progress, swipe up the build status bar at the bottom of your screen.

Once the sync is successful, you can start working on your project or simply press the Run button in the toolbar to build and install your application.

LOVE WHAT YOU SEE?
logo
AndroidIDE.
© 2021-2023 AndroidIDE

SOCIALS
Installation
Getting Started
UI Designer

Editor
AndroidIDE

logo


The UI Designer
The UI Designer helps you visually design XML layouts by simply dragging and dropping widgets into the workspace.

This document briefly explains every element of the UI Designer workspace.

The workspace
Your XML code is parsed and inflated by AndroidIDE's LayoutInflater API and then shown in the workspace. You can drag and drop the inflated views and widgets to move them, change their attributes, add new views or delete the existing ones.

Workspace
Drag-n-Drop

Add new views
To add new views into the workspace:

Open the left drawer which shows a list of supported views and layouts.
Long click on the list items to start the drag. Drop them into the workspace to add to the layout.
To move a view in the workspace, you can simply long press the view to start the drag and then drop it at the desired position.

Widget drawer

Edit view attributes
Clicking on any inflated view opens the view info sheet which contains information about the view.

The sheet contains two buttons at the header :

Add - Shows a list of attributes that you can add to the selected view. The list does not contain attributes that have been already applied to the view.
Delete - Deletes the selected view.
It also contains the list of attributes that have been applied to the selected view.

Clicking on any attribute opens the value editor which you can use to edit the value of the selected attribute.
Clicking on the 'Delete' button next to the attribute deletes that attribute from the view. However, some necessary attributes cannot be deleted (android:layout_height and android:layout_width for example).
View info sheet

The layout hierarchy
When views are invisible in the workspace (height or width is set to 0), it makes it harder to edit the properties/attributes of those views. This is where the layout hierachy view comes in. It shows the layout hierarchy of the views that are shown in the workspace in a tree-like structure.

You can open the layout hierarchy by simply opening the right drawer or clicking on the 'hierarchy' view in the options menu. Clicking on the nodes of the tree is same as clicking on the views in the workspace (opens up the view info sheet).

See screenshot
LOVE WHAT YOU SEE?
logo
AndroidIDE.
© 2021-2023 AndroidIDE

SOCIALS
Installation
Getting Started
UI Designer

Editor
AndroidIDE
