# Annotation Processor Tool for DroiBaaS SDK
An APT provides you to generate helper class for DroiBaaS. 


# Installation

## Android Studio

1. Enable APT feature in Android Studio

	```ruby
	repositories {
		mavenCentral()
		maven {
			url "https://github.com/DroiBaaS/DroiBaaS-APT-Android/raw/master/"
		}
	}

	```

2. Add APT maven repository

	```ruby
	buildscript {
		repositories {
			mavenCentral()
		}
		dependencies {
			classpath 'com.android.tools.build:gradle:1.3.0'
			classpath 'com.neenbedankt.gradle.plugins:android-apt:1.8'
		}	
	}
	
	apply plugin: 'android-apt'
	```
	
3. Add dependencies

	```ruby
	dependencies {
		...
		apt 'com.droi.sdk:annotationprocessor:+'
		...
	}
	```
