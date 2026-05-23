# Building Your Game

## Strip Unused Resources Folders

By default, Unity will include the content of any folder named "Resources" in your build.  Since all the demo games use _Resources_ folders, it is important to strip them before building, or their content will end up being included in your build, increasing its size.

To strip the demo games, open the Welcome Window by clicking **Tools -> AnyRPG -> Welcome Window** and click on the STRIP ALL DETECTED DEMO GAMES button.

<figure><img src="../.gitbook/assets/image (183).png" alt=""><figcaption></figcaption></figure>

## Build The Game

Open the Build Profiles window from the main toolbar by clicking **File -> Build Profiles**.  Ensure the build profile for your game is active, and ensure that the game loading scene is the first scene in the list.  Click _Build_ or _Build and Run_.

<figure><img src="../.gitbook/assets/image (184).png" alt=""><figcaption></figcaption></figure>

## Next Steps

Reference [Unity build profile documentation](https://docs.unity3d.com/6000.3/Documentation/Manual/build-profiles.html) to learn more about builds in Unity.
