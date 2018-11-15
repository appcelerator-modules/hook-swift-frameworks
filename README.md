# Swift iOS Frameworks in Titanium
Support Swift frameworks in native Titanium modules.

### Prerequisites
- [x] Titanium SDK 6.2.0+ (to support dynamic libraries in general)
- [x] Swift framework that exposes an Objective-C public-header

### Usage
1. Download the `ti.swiftsupport.js` file and open it
2. Search for the `SWIFT_VERSION` variable and specify your Swift version used [[*](#note-1)]
3. Adjust your module project code by placing the `ti.swiftsupport.js` file in `<your-module-ios-root>/hooks`
5. That's it!

##### Note 1: 
This is required since Swift currently does not have ABI-stability which is expected to be supported in future versions of Swift. Until then, you always need to use the Swift version that the framework was compiled with.

##### Note 2:
If you use Hyperloop, you can add this as a project level hook. To do so simply place the `ti.dynamiclib.js` file in `<your-project-root>/hooks`

### License
Apache 2.0

### Legal
This module is Copyright (c) 2017-present by Axway Appcelerator. All Rights Reserved. Usage of this module is subject 
to the Terms of Service agreement with Axway, Inc. 

### Contributing
Code contributions are greatly appreciated, please submit a new [Pull Request](https://github.com/appcelerator-modules/hook-swift-frameworks/pull/new/master)!
