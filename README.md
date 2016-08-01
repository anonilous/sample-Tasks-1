# Tasks sample application
Open source cross-platform Tasks app built with NativeScript.

Use this application to find-out how to implement common mobile scenarios with NativeScript.
![](https://d2odgkulk9w7if.cloudfront.net/images/default-source/default-album/07-2-signupd66b612a7b776b26a649ff00000922f2.png?sfvrsn=1)
![](https://www.nativescript.org/images/default-source/default-album/sample-tasks-list.png)
![](https://d2odgkulk9w7if.cloudfront.net/images/default-source/default-album/03-editnewtaskbc6b612a7b776b26a649ff00000922f2.png?sfvrsn=1)
![](https://www.nativescript.org/images/default-source/default-album/sample-tasks-details.png)

## Running the sample

1. Make sure you have the [NativeScript Command-line Interface](https://www.npmjs.com/package/nativescript) installed as well as all the prerequisites for the NativeScript development, described in the package page.

2. Install the dependencies of the sample (NativeScript modules and TypeScript compiler)

       `npm install`

3. Compile the TypeScript code

       `node_modules/typescript/bin/tsc -p ./app`

4. Add the preferred platform-specific tools to the project library. Note that iOS development is only available with a Mac machine.

    `tns platform add ios|android`

5. [Android only] Copy the AndroidManifest.xml file to the Android project folder.

    `cp ./manifests/AndroidManifest.xml ./platforms/android/src/main`

4. Run the project.

    `tns run ios|android [--emulator]`

    The `--emulator` keyword instructs the CLI to load the iOS simulator or an android emulator depending on the platform you want.


For convenience you can use the `run.bat`/`run.sh` scripts on a \*NIX/windows environment respectively. The `run.sh` script starts the sample in iOS when run on a Mac and Android on Linux/Windows. The `run.bat` script runs the sample on an Android emulator under Windows.

For \*NIX systems the following script runs the sample directly:

`curl https://raw.githubusercontent.com/NativeScript/sample-Tasks/master/run.sh | bash`


## Application Scenario

We chose an app that we know will cover a lot of useful scenarios:

1. User management
  1. User authentication
  2. User registration
  3. User welcome email

2. Cloud data 
  1. read, update, delete and create data entry stored in the cloud
  2. Offline support for the data (not in this article, but coming soon)

3. Modern UX
  1. Using SideBar
  2. Pull to Refresh
  3. FAB (floating action button for Android Lollipop)
  4. Load on demand for many tasks

4. Device integration
  1. using camera
  2. using phone contacts

5. Patterns/Technologies used
  1. MVVM 
  2. CSS for styling
  3. XML and data-binding for describing the UI
  4. Platform specific targeting for the Android FAB button       
  5. 3rd party native libraries to load Telerik UI

Please read the series of articles that explain how this application is being implemented - https://www.nativescript.org/blog/nativescript-open-source-sample---tasks


