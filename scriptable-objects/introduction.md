# Introduction

The AnyRPG Engine makes heavy use of [Unity Scriptable Objects](https://docs.unity3d.com/Manual/class-ScriptableObject.html) to allow as much configuration of games as possible without requiring changes to the engine code.

## Properties

All scriptable objects used in AnyRPG have a common set of shared properties.  To avoid duplication in the documentation, they are all listed here.  Individual scriptable object pages will only list additional properties that are not on this page.

| Name                         | Description                                                                                                                                                                                                       |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Resource Name                | The resource name serves as a database key when scriptable object lookups are performed in the engine.  If the _Display Name_ field is empty, it will also be the display text wherever the item appears in-game. |
| Display Name                 | The display name field can be used when a different display text than the _Resource Name_ is desired, or when using localization to display text in different languages.                                          |
| Icon                         | Whenever the UI will show an image for a certain scriptable object, this icon will be used.                                                                                                                       |
| Icon Background Image        | <p>If an icon is transparent, this image will show behind the icon.<br>This can be useful to reduce effort and save space, by re-using background images for multiple icons.</p>                                  |
| Description                  | Whenever the UI shows a description for a scriptable object, this text will be displayed.                                                                                                                         |
| Use Regional Description     | If true, the system will search for a localized regional description for this scriptable object and use its _Display Name_, _Icon_, _Icon Background Image_, and _Description_ instead.                           |
| Resource Description Profile | If set, the system will search for a regional description with this name for this scriptable object and use its _Display Name_, _Icon_, _Icon Background Image_, and _Description_ instead.                       |
| Optional Override            | If true, and one of the two regional override fields is used, the regional override is optional, and will not cause an error if it doesn't exist.                                                                 |

