## Notes

- This builds an empty SwiftUI project created in Xcode on EAS. I haven't tried doing the equivalent for Android yet
- I renamed the directory containing the iOS project to **ios** to play nicely with EAS tooling
- Note to self: I had to run the build in Xcode once after initializing it in order for Xcode to created the **xcshareddata** folder, which we use to find build schemes
- You can run the build with `eas build --profile development` - this will create simulator build, following the build steps from **.eas/build/simple.yml** ([example build](https://expo.dev/accounts/brents/projects/builds-example/builds/1b191d4a-82ef-41d1-a8ca-0158a8053ca9) - requires iOS 17.5+ simulator to run)
- EAS CLI will produce a few warnings:

```
✔ Uploaded to EAS
Failed to read app versions.
Failed to locate Info.plist files relative to path "/Users/brent/code/builds-example".
Please report this as an issue on https://github.com/expo/expo/issues
Proceeding anyway..
```