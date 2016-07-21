# DroiCoreSDK 
A library provides you to use powerful DroiBaaS cloud service from your Android app. DroiCore SDK is foundation library of DroiBaaS. For more information, see [DroiBaaS](https://github.com/DroiBaaS/DroiBaaS-SDK-Android).

# Using DroiCoreSDK

## Installation

### Android
The easiest way to use DroiCoreSDK is with gradle. Add the following lines to your `build.gradle`.

1. Add DroiCoreSDK maven repository

	```ruby
	repositories {
		mavenCentral()
		maven {
			url "https://github.com/DroiBaaS/DroiBaaS-SDK-Android/raw/master/"
		}
	}

	```
	
2. Add dependencies

	```ruby
    compile 'com.squareup.okhttp3:okhttp:3.0.1'
    compile 'com.droi.sdk:droi-baas-android-sdk:+'
	```

## Using DroiCoreSDK in your Android code

1. Add `ApplicationID`, `PlatformID` and `ChannelID` into your AndroidManifest.xml

	```
<meta-data android:name="com.droi.sdk.application_id" android:value="[DroiBaaS Application ID]" />
<meta-data android:name="com.droi.sdk.platform_key" android:value="[DroiBaaS ClientKey]" />
<meta-data android:name="com.droi.sdk.channel_name" android:value="[ChannelName]" />
	```
	
2. Before using any DroiCoreSDK, please call `Core.initialize(this);` first.

# Example Project
