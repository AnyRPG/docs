---
description: >-
  The minimap wizard creates a top down image of a scene to be used for the main
  map and minimap.
---

# Minimap Wizard

{% embed url="https://youtu.be/SqGLSVgY528" %}

## Accessing the Wizard

The minimap wizard requires that the game scene you want to make the map for is open in the editor.  The scene should have a SceneConfig object in it to work properly.

The Minimap Wizard can be opened by clicking _Tools_ in the menu bar, and selecting _AnyRPG > Wizard > Minimap Wizard_.

![](<../.gitbook/assets/image (8).png>)

![](<../.gitbook/assets/image (1) (1) (1).png>)

## Settings

| Name               | Description                                                                                                                                                                                                                                           |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Game Name          | The name of the game in your Unity project to install the template content in.  This will be automatically filled in if you have any scene with the SceneConfig prefab open.                                                                          |
| Pixels Per Meter   | The number of pixels to be rendered in the map image per horizontal meter of the scene.                                                                                                                                                               |
| Camera Clear Flags | <p><strong>Depth</strong><br><strong></strong>The image will have a transparent background<br><strong>Color</strong><br>The image will have a solid color background<br><strong>Skybox</strong><br>The image will have a skybox in the background</p> |
| Background Color   | If the geometry of the level is not a perfect square, and the Camera Clear Flags are set to color, what color should be used to fill in the empty areas.                                                                                              |

## Content Created

After choosing all the settings, click Create to run the wizard.

![](<../.gitbook/assets/image (32).png>)

The following content will be created.

### Map Image

The map image can be found in the _GameName/Images/MiniMap_ folder.

![](<../.gitbook/assets/image (38).png>)

## Next Steps

The minimap image will be loaded automatically when the scene is loaded.  There is no additional configuration required.
