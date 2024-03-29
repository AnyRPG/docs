---
description: >-
  The AnyRPG Core package is available via github and the Unity Asset Store.
  This page describes how to install it from github.
---

# Github Installation

## Install the Correct Unity Version

The AnyRPG Unity package is exported as a complete project because it requires specific build settings, compiler settings, layers, and tags to function. Due to the way full projects are exported in Unity, they must be imported with the **same** Unity version they were exported with.

The correct Unity Version for the current github project is 2021.3.11f1 and can be downloaded from [ https://unity3d.com/get-unity/download/archive](https://unity3d.com/get-unity/download/archive)\


## Download the Project From Github

Choose one of the download methods that Github offers.\
![](<../../.gitbook/assets/image (8).png>)

For example, you can clone the project into a directory on your computer if you have the git CLI installed using the command `git clone git@github.com:AnyRPG/AnyRPGCore.git`

![](<../../.gitbook/assets/image (16).png>)

## Open Unity Hub and Add the Project

Open Unity Hub and select the _Projects_ tab.  Click _Open > Add Project From Disk._

![](<../../.gitbook/assets/image (15) (2).png>)

Find the project folder and choose _Add Project_.

![](<../../.gitbook/assets/image (12).png>)

## Open The Project

The project should now be visible in Unity Hub.  Click on it to open it.

![](<../../.gitbook/assets/image (3) (2).png>)

When presented with the option, choose Ignore.  This is necessary because AnyRPG relies on UMA and it's not included in the github project.

![](<../../.gitbook/assets/image (21).png>)

Once the project opens, you will see errors in the console.  These will be fixed in the next step by installing UMA.

![](<../../.gitbook/assets/image (22) (2).png>)

## Install UMA 2

Install UMA 2 from the Unity Asset Store at [https://assetstore.unity.com/packages/3d/characters/uma-2-unity-multipurpose-avatar-35611](https://assetstore.unity.com/packages/3d/characters/uma-2-unity-multipurpose-avatar-35611)

If you don't already own UMA, click _Add to My Assets_.

![](<../../.gitbook/assets/image (10) (3).png>)

Click _Open in Unity_.

![](<../../.gitbook/assets/image (24).png>)

The Unity Package Manager should open in Unity.  If you have not downloaded the package yet, click _Download_.  Then Click _Import_.

![](<../../.gitbook/assets/image (1) (2) (4) (1).png>)

When presented with the option, accept the defaults and click Import.

![](<../../.gitbook/assets/image (20).png>)

Since UMA has not been updated to the new 2021 API yet, you will have to accept the script update.  Click _Yes, just for these files_.\
![](<../../.gitbook/assets/image (2) (8) (1).png>)

After the UMA package is imported, click Clear in the Console pane to clear any old warnings.

![](<../../.gitbook/assets/image (7).png>)

You should no longer see any errors.

![](<../../.gitbook/assets/image (17).png>)

Finally, rebuild the UMA Global Library.  Choose from the main menu bar _UMA > Global Library_.

![](<../../.gitbook/assets/image (99).png>)

In the Global Library window, choose _File > Rebuild From Project_.

![](<../../.gitbook/assets/image (18).png>)

## Install TMP Essental Resources

Open the Window menu in Unity and choose _TextMeshPro > Import TMP Essential Resources_.

![](<../../.gitbook/assets/image (4) (2).png>)

When presented with the option, accept the defaults and click **Import**.

![](<../../.gitbook/assets/image (3).png>)

## Next Steps

Congratulations, AnyRPG is now ready to use!

From here you can explore the [included sample games](../included-sample-games.md) or get started [creating your own game](../creating-your-first-game.md).
