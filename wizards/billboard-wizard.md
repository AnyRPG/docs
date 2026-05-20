---
description: >-
  The Billboard Wizard helps you quickly make a billboard from a tree to use
  with LOD.
---

# Billboard Wizard

## Accessing the Wizard

The Billboard Wizard is designed to make billboards of 3D models that can be used for LOD.  The recommended workflow is to open a 3D model prefab in the Unity Editor before accessing the wizard.

The Billboard Wizard can be opened by clicking _Tools_ in the menu bar, and selecting _AnyRPG > Wizard > Billboard Wizard_.

<div align="left"><figure><img src="../.gitbook/assets/image (162).png" alt=""><figcaption></figcaption></figure></div>

## Making a Billboard

By default, the billboard wizard will show a white indicator square in the scene view window.  This square represents the size and contents of the image that will be saved to disk.

You can adjust the background of the image, and the lighting that will be used when the screenshot is taken, but those settings will not show in the scene view.  You may have to take a few screenshots to get the settings just right.  A full list of the settings can be found below.

It is recommended to use the orientation tool to ensure the item fits in the image frame from all sides.

<div align="left"><figure><img src="../.gitbook/assets/image (165).png" alt=""><figcaption></figcaption></figure></div>

Once you are satisfied with the settings, click the _Create_ button and the a billboard will be created.

<figure><img src="../.gitbook/assets/image (164).png" alt=""><figcaption></figcaption></figure>

## Settings

| Name                | Description                                                                                                                                                              |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Parent Folder       | The folder that the billboard will be saved in, relative to the Assets folder in your project.                                                                           |
| File Name           | The name of the file that will be saved to disk.  If a file of the same name exists, the file name will have the current date and time appended to it to make it unique. |
| Show Size Indicator | If true, a white indicator square will show on screen to represent the size and contents of the screenshot.                                                              |
| Width               | The width of the output image                                                                                                                                            |
| Height              | The height of the output image                                                                                                                                           |
| Use Light           | If true, a light will be attached to the camera that takes the screenshot, emulating the settings you see in the scene view.                                             |
| Light Color         | If _Use Light_ is selected, the color of the light to shine on the object.                                                                                               |
| Light Intensity     | If _Use Light_ is selected, the brightness of the light to shine on the object.                                                                                          |

