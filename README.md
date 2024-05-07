# edgegap-unity-plugin

Source Code for Unity Plugin for Edgegap Integration
More information can be found on [Edgegap Documentation](https://docs.edgegap.com/docs/tools-and-integrations/unity-plugin)

# v2

This fork introduces an improved UI for the Edgegap Manager:

![Edgegap Settings Manager](https://i.imgur.com/ttH338r.png)

**Not Yet Implemented:**

1. Build & Push button click
2. Deployments group
3. Persistence
4. Manage existing apps

## Installing the package

### From Unity store

~~You can add to your Assets the latest published version from the [**Unity Asset Store**](https://assetstore.unity.com/packages/tools/network/edgegap-cloud-server-212563)
and import it with the Package Manager under `Window > Package Manager` then selecting `My Assets` as the source.~~

Asset store version is temporarily out of order, we apologize for the inconvenience. Stay tuned for updates.

### From Source

1. Git clone this project [https://github.com/edgegap/edgegap-unity-plugin](https://github.com/edgegap/edgegap-unity-plugin)

   `git clone https://github.com/edgegap/edgegap-unity-plugin`

2. Open the project with Unity Hub

3. Export the package under `Assets > Export Package...` and remove the default scene from the selection.

4. Save the `.unitypackage`

5. In your Unity Editor, go to `Assets > Import Package > Custom Package...` and navigate to the `.unitypackage` file.

6. You will see a window with the various files that are about to be imported into your project.
   Everything under `Edgegap` is related to our server management tool, and under `Plugins` is the `dll` file for `Newtonsoft.Json`.

   If you already have this plugin installed in your project, or if your Unity version is above 2019.4, you should **not** import the `Plugins`
   folder to avoid duplicates and conflicts in your project files.

   If your Unity version is 2019.4 and you don't already have `Newtonsoft.Json` in your project, keep the `Plugins` folder selected.
