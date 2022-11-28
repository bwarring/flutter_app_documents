# flutter_app_documents
Repository for containing documentation, images, and videos for mobile applications.  Can be referenced in README.md files.

# FLUTTER PUBLISH ANDROID APK
## ANDROID DEPLOYMENT

* [docs.flutter.dev - Android Deployment](https://docs.flutter.dev/deployment/android)
### [BUILD AN APK](https://docs.flutter.dev/deployment/android#build-an-apk)<br>
Small snippet from document:
  
```
* Enter cd [project]
* Run `flutter build apk --split-per-abi`<br>
(The flutter build command defaults to --release.)
  
This command results in three APK files:

1. [project]/build/app/outputs/apk/release/app-armeabi-v7a-release.apk
2. [project]/build/app/outputs/apk/release/app-arm64-v8a-release.apk
3. [project]/build/app/outputs/apk/release/app-x86_64-release.apk

  
Removing the `--split-per-abi` flag results in a fat APK that contains your code compiled for all the target ABIs. Such APKs are larger in size than their split counterparts, causing the user to download native binaries that are not applicable to their device’s architecture.
```
  
### [INSTALL APK ON ANDROID DEVICE](https://www.groovypost.com/howto/install-apk-files-on-android/)
Load one of the `*.apk` files listed above.  Which file to load depends on what kind of processor is running on your device.  If you don't know what kind of processor is running on your device, then unfortunately that system information is not available in most, if not all, device settins.  The link in this section heading recommends
* [Droid Hardware Info](https://play.google.com/store/apps/details?id=com.inkwired.droidinfo)
<br>
  
<img src="https://github.com/bwarring/flutter_app_documents/blob/main/flutter/images/droid-hardware-info%2001.jpg?raw=true" alt="note" width="280"/>&nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://github.com/bwarring/flutter_app_documents/blob/main/flutter/images/droid-hardware-info%2002.jpg?raw=true" alt="note" width="280"/>
  
The kind of processor is identified in `Instruction Sets` property under the `System` tab.  Select appropriate APK based on `Instruction Sets` value(s).