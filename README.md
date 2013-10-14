ZingMeSDK
=========
Zing Me SDK For iOS

Getting Started

The ZingMe SDK for iOS is designed to be easy to install and use. This guide walks through the basics of setting up the development and project environment and creating a simple app.
Watch the screencast or follow the steps below.
1. Install the Prerequisites
OS X is required for all iOS development. If you're completely new to iOS development, you'll need to install Xcode from the App Store.


2. Install the ZingMe SDK for iOS
Download the SDK here and install the package. The default install location is ~/Documents/ZingMeSDK.
Source code for the SDK is also available on the link 

3. Run the Samples
The SDK includes a ZingMeSDKTest sample that include all of features of SDK.
4. Create a Facebook App
Configure a new Xcode Project
In Xcode, create a new project, and select 'Single View Application' as shown below.
 
Provide a name and identifier as required:

Add the ZingMe SDK & Bundle resource 
The ZingMe SDK for iOS is a framework that you add to your Xcode project. 
To add the SDK, open ~/Documents/ZingMeSDK and drag the ZingMeDSK.framework folder into the Frameworks section of your Project Navigator.

Choose 'Create groups for any added folders' and deselect 'Copy items into destination group's folder (if needed)' to reference the SDK where it was installed rather than copying the SDK into your app.
To add bundle resource, open ~/Documents/ZingMeSDK/ ZingMeSDK.framework/Resources/ ZingMeSDKResources.bundle and drag the ZingMeSDKResources.bundle file into the Frameworks section of your Project Navigator.
 
Choose 'Create groups for any added folders' and deselect 'Copy items into destination group's folder (if needed)' to reference the Bundle where it was installed rather than copying the Bundle into your app.

Configure your project
Add more framework:You need add Security.framework and MessageUI.frameword to your Xcode project by select Link Binary With Libraries in Build Phases in your Xcode project setting as picture below.
 
Setting Other Linker Flags
Add “-all_load” to Other Linker Flags by select Builds Settings and find the Other Linker Flags property and add “-all_load” flag to this property as picture below.
 
Add some properties to AppDelegate
Finally, you need to add some properties to AppDelegate as picture below
NSString* kAppName          = @"ulabs_vuibanca";
     NSString* kApiKey           = @"c79c78a4233d40c7bb65d388f228ee8e";
    NSString* kApiSecret        = @"227ba82b951b4252b58956b7286c4e22";
     NSString *kAppId            = @"ulabs_vuibanca";
    #warning TODO: change Language
  NSString *kLanguage         = @"vi”; //vi: Tieng viet  en: Tieng anh
 

Thats it! Now you can start coding your iOS app with ZingMe.
