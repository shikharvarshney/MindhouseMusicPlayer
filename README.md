# MindhouseMusicPlayer - Music Player App

I have tried to provide all the necessary pre-requisites in this project which can allow any fellow developer to follow this. The constitues of the project and instructions for 'How to install?' are mentioned later in this document.
Here is the video link to show how the app is working:- https://mindhousemusicplayerapp.s3.amazonaws.com/MindhosueMusicPlayerApp.mp4

### Note:- 
The Api was not returning the description key for every item, therefore I have decided to use static text in the detail screen instead of reading the text from API.

### Prerequisites

What things you need to install the software and how to install them

```

Software	          Version
Android studio (IDE)	>= 2.2.3
Android Sdk	        >= 25.0.2
Java	                >= 1.8.0_121
Node Js	                >= 8.0
React native cli        2.0.1
Cocoapods               Install the latest one
Homebrew                Install the latest one
XCode                   >= 11.0
Yarn                    Required, it is a good practice to install yarn for latest React Native versions.
Any Editor of your      Latest Version
Choice. Preferably 
VSCode
```

## What all is there in this template?

1. It is on latest ```React Native version 0.63.4``` in which autolinking is supported.
2. ```Splash Screen with Lottie Animation```.
3. A highly intuitiuve design has been tried to implement here as per your instructions.
4. No ```Redux methodology``` is followed in this project and I have tried to experiment with a new Pub-Sub pattern to maintain state.
5. ```Lottie package``` is already installed in the project for enhancing the Look of aniamtions.
6. ```Basic Navigation stack``` using React Navigation 5 is already done in the project. 
7. ```Linting rules``` has already been defined as per latest ```Airbnb guidelines```. Install Prettier in your VSCode and set the rules defined in .eslintrc file.
8. All the other Animations like ```Sticky header``` on scrolling the main screen have been implemnted using Native Driver for smoothness.
9. All the managament of Code Structure, Folder Structure, Design Pattern, Fonts, Images have been properly managed in the project. Just follow the best practices and you will never have to worry about anything else.
15. I have tried to make Reusable components so that they can be used independently in the project to maintain consistency. You can also tweak them as per your need.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.



### Installing

```
Step 1:-
```
Clone the Github Repo either by using HTTPS or SSH onto your local machine using the command "git clone". The master branch will be cloned to your project.

```
Step 2:- 
```
Checkout the branch ```main``` using the command ```git checkout <branch-name>```.

```
Step 3:- 
```
cd into the root directory of the project and do ```yarn install```.

```
Step 4:- 
```
cd ios and the type the command ```pod install```.

```
Step 5:- 
```
Either open the project in respective IDEs like XCode (<project-name>.xcworkspace file) or Android Studio(android folder) and run the project from there only OR run the following commands ```react-native run-ios``` or ```react-native run-android``` from your terminal window from the root directory of your project to start the project.
    
    
## Common Pitfalls and Errors while Installing the Project and how to solve them.

I have tried our level best that by folowing the above steps you can directly get the project running without any hustle. However there may be some probable issues while trying to run the project based on the individual system configs. Here are possible scenarios and how to remove them.

1. If you face any error for ```-darwin flag``` then please update the version of ```Flipper-Folly``` and ```OpenSSL-Universal``` to 1 above. I have downgraded it to 1 version as I have been using Xcode 11.3.1. Please refer this link:- https://github.com/facebook/react-native/issues/30231
2. Pods not getting installed or Cocoapods version is an older one:- Please install Cocoapods first and if it is present then update it to latest version.
3. Some error with Pods:- Please remove the `Pods Folder` and `podfile.lock` from the `ios` directory either manually or by typing these commands from terminal ```rm -rf Pods && rm -rf podfile.lock``` and then perform a fresh `pod install`.
4. If there is a error regarding starting the metro bundler due to javascript and node version mismatch:- Please run this following command ```watchman watch-del-all && react-native start --reset-cache```.
5. If ```watchman``` is not installed then please install it first by typing the following command ```brew install watchman```.

    
## Contributors
* **Shikhar Varshney**

## Acknowledgments
* **Dribbble**
