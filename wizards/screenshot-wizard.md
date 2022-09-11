---
description: The Screenshot Wizard helps you quickly make icons of any 3D model.
---

# Screenshot Wizard

{% embed url="https://youtu.be/s9vRImPeG4g" %}

## Accessing the Wizard

The Screenshot Wizard is designed to make icons of 3D models.  The recommended workflow is to open a 3D model prefab in the Unity Editor before accessing the wizard.

The Screenshot Wizard can be opened by clicking _Tools_ in the menu bar, and selecting _AnyRPG > Wizard > Screenshot Wizard_.

![](<../.gitbook/assets/image (33).png>)

![](<../.gitbook/assets/image (81).png>)

## Making an Icon

By default, the screenshot wizard will show a white indicator square in the scene view window.  This square represents the size and contents of the image that will be saved to disk.

![](<../.gitbook/assets/image (22).png>)

You can adjust the background of the image, and the lighting that will be used when the screenshot is taken, but those settings will not show in the scene view.  You may have to take a few screenshots to get the settings just right.  A full list of the settings can be found below.

It is recommended to experiment with the rotation of the item to ensure the most distinct or unique feature takes up the full frame of the size indicator preview.

Once you are satisfied with the settings, click the _Create_ button and the image will be saved to disk.

![](<../.gitbook/assets/image (48).png>)

![](<../.gitbook/assets/image (59).png>)

Don't forget to open the saved image in the inspector and set the _Texture Type_ to _Sprite (2D and UI)_ so you can use the image as an icon.

![](<../.gitbook/assets/image (40).png>)

## Settings

| Name                  | Description                                                                                                                                                                                                                                           |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Parent Folder         | The folder that the screenshot image will be saved in, relative to the Assets folder in your project.                                                                                                                                                 |
| File Name             | The name of the image file that will be saved to disk.  If a file of the same name exists, the file name will have the current date and time appended to it to make it unique.                                                                        |
| Show Size Indicator   | If true, a white indicator square will show on screen to represent the size and contents of the screenshot.                                                                                                                                           |
| Width                 | The width of the output image                                                                                                                                                                                                                         |
| Height                | The height of the output image                                                                                                                                                                                                                        |
| Camera Clear Flags    | <p><strong>Depth</strong><br><strong></strong>The image will have a transparent background<br><strong>Color</strong><br>The image will have a solid color background<br><strong>Skybox</strong><br>The image will have a skybox in the background</p> |
| Background Color      | If the Color option is chosen for the _Camera Clear Flags_, this is the color that will be used.                                                                                                                                                      |
| Use Light             | If true, a light will be attached to the camera that takes the screenshot, emulating the settings you see in the scene view.                                                                                                                          |
| Light Color           | If _Use Light_ is selected, the color of the light to shine on the object.                                                                                                                                                                            |
| Light Intensity       | If _Use Light_ is selected, the brightness of the light to shine on the object.                                                                                                                                                                       |
| Object To Screen Shot | Although the screenshot will take a picture of whatever is shown in the size indicator, the camera must be attached to some prefab in the scene view.  This setting controls what object the camera is attached to.                                   |

