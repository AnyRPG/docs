---
description: >-
  The AnyRPG Core package is available via github and the Unity Asset Store.
  This page describes how to install it from from the Unity Asset Store.
---

# Unity Asset Store Installation

{% embed url="https://youtu.be/syI3ohFWVck" %}

## Find AnyRPG Core on the Unity Asset Store

AnyRPG Core can be found on the Unity Asset Store at [https://assetstore.unity.com/packages/slug/234361](https://assetstore.unity.com/packages/slug/234361)

## Install the Correct Unity Version

The AnyRPG Unity package is exported as a complete project because it requires specific build settings, compiler settings, layers, and tags to function. Due to the way full projects are exported in Unity, they must be imported with the **same or higher** Unity version they were exported with.

You can find the correct Unity version right on the asset store page.\


![](<../../.gitbook/assets/image (1) (1).png>)

## Create a New Unity 3D Project

Open Unity Hub and select the _Projects_ tab.  Click _New project_.

![](../../.gitbook/assets/Untitled.png)

If you have multiple versions of Unity installed, you will need to select the correct editor version.  Choose 3D (URP/HDRP are not available yet), optionally name your project, and click the _Create project_ button.

![](<../../.gitbook/assets/image (89).png>)

## Install the AnyRPG Unity Package

Add the AnyRPG Core asset to your assets by clicking the **Add To My Assets** button on the asset store page.

![](<../../.gitbook/assets/image (22).png>)

Once the asset is added to your assets, click the **Open in Unity** button.

![](<../../.gitbook/assets/image (15).png>)

When the package manager opens in Unity, click the Download button to download the package.

![](<../../.gitbook/assets/image (4).png>)

Once the package has downloaded, the **Import** button should become available.  Click it.

<img src="../../.gitbook/assets/image (3).png" alt="" data-size="original">

A warning window will pop up letting you know this package will overwrite all project settings.  Click **Import**.

![](<../../.gitbook/assets/image (5).png>)

A warning window will pop up prompting you to upgrade package manager dependencies.  This is necessary to ensure that packages that AnyRPG relies on, such as the Post Processing package are installed.  Click **Install/Upgrade**.

![](<../../.gitbook/assets/image (1) (2).png>)

When the Import Unity Package window appears, click **Import**.

![](<../../.gitbook/assets/image (98).png>)

The AnyRPG Unity package contains hundreds of textures, icons, 3d models, and audio files.  You can expect the import to take a few minutes, even on a reasonably fast computer.

![](<../../.gitbook/assets/image (34).png>)

Once the import completes, you will see errors in the console.  These will be fixed in the next step by installing UMA.

![](<../../.gitbook/assets/image (22) (2).png>)

## Install UMA 2

Install UMA 2 from the Unity Asset Store at [https://assetstore.unity.com/packages/3d/characters/uma-2-unity-multipurpose-avatar-35611](https://assetstore.unity.com/packages/3d/characters/uma-2-unity-multipurpose-avatar-35611)

If you don't already own UMA, click _Add to My Assets_.

![](<../../.gitbook/assets/image (10).png>)

Click _Open in Unity_.

![](<../../.gitbook/assets/image (24).png>)

The Unity Package Manager should open in Unity.  If you have not downloaded the package yet, click **Download**.  Then Click **Import**.

![](<../../.gitbook/assets/image (1) (2) (4).png>)

When presented with the option, accept the defaults and click **Import**.

![](<../../.gitbook/assets/image (20).png>)

Since UMA has not been updated to the new 2021 API yet, you will have to accept the script update.  Click **Yes, just for these files**.\
![](<../../.gitbook/assets/image (2) (8).png>)

After the UMA package is imported, click **Clear** in the Console pane to clear any old warnings.

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

{% hint style="warning" %}
AnyRPG Includes a modified version of the Liberation Sans SDF Asset so be sure to **uncheck** the box beside AnyRPG before clicking _Import_.
{% endhint %}

![](<../../.gitbook/assets/image (23).png>)

## Next Steps

Congratulations, AnyRPG is now ready to use!

From here you can explore the [included sample games](../included-sample-games.md) or get started [creating your own game](../creating-your-first-game.md).
