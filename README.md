## Project Installation
### 1. Git checkout / clone project
```sh
$ git clone https://github.com/ArshadRayeen/rn-project-structure.git <ProjectName>
$ cd <ProjectName>
```
### 2. Rename Project  
```sh
$ yarn global add react-native-rename
                  or
$ npm install react-native-rename -g
```
`ignore if already installed`
```sh
$ npx react-native-rename <ProjectName> -b <bundleIdentifier>
```
### 3. Install node modules / libraries
```sh
$ yarn  
    or  
$ npm install
```
### 4. Pod install
```sh
npx pod-install ios
```
### 5. Run Project

Run the following command in a Terminal at root of source directory:

```sh
$ npx react-native run-ios          // for iOS
        OR
$ npx react-native run-android      // for Android
```

## Change git repository & initial commit 
Run the following commands in a Terminal at root of source directory:

### 1. Remove git folder
```sh
$ rm -rf .git
```
### 2. Add git repo 
```sh
$ git init
$ git remote add origin https://<username>@gitlab.com/<repo>.git
```
### 3. Inital commit
```sh
$ git add .
$ git commit -m "inital commit"
```
### 3. Push code into origin git server
```sh
$ git push --force origin master
```

README.md
------------ 

# {APP_NAME} Mobile App
This is the JavaScript and React Native source code for {APP_NAME} Mobile App.


## Installation
You will need Node, Watchman, React Native CLI, Xcode, and CocoaPods.

### Node, Watchman

We recommend installing Node, Yarn, and Watchman using Homebrew. Run the following commands in a Terminal after installing Homebrew:

```sh
$ brew install node
$ brew install watchman
```

If you have already installed Node on your system, make sure it is Node 10.11.0 or newer.

If you get an error like `Cannot find module 'npmlog'`, try installing npm directly: `curl -0 -L https://npmjs.org/install.sh | sudo sh`.


### CocoaPods

CocoaPods is built with Ruby and is installable with the default Ruby available on macOS. We recommend you use the default ruby.

```sh
$ sudo gem install cocoapods
```
### Dependencies

Run the following commands in a Terminal at root of source directory:

``` bash
$ cd {APP_NAME}
$ yarn
$ npx pod-install ios
```

## Run

Run the following command in a Terminal at root of source directory:

```sh
$ npx react-native run-ios          // for iOS
        OR
$ npx react-native run-android      // for Android
```

`npx react-native run-ios` or `npx react-native run-android` is just one way to run your app. You can also run it directly from within Xcode and Android Studio respectively or [Nuclide](https://nuclide.io/). You can refer [React Native Get Started](https://reactnative.dev/docs/getting-started) guide for more info.
