# Flutter Playground
Playground app for Flutter.
Contains list examples that Bhavik Makwana has created.

[Resource1:](https://blog.geekyants.com/project-hummingbird-32d642eed30c)
[Resource2:](https://flutter.dev/docs/get-started/install/macos)
[Resource3:](https://app.codacy.com/app/ibhavikmakwana/FlutterPlayground)
[Resource4:](https://github.com/flutter/flutter_web)
[Resource5:](https://flutter.github.io/samples)


## Getting Started
For help getting started with Flutter, view online
[documentation](https://flutter.io/).

## Visual Studio Code
Visual Studio Code supports Flutter web development with the v3.0 release of the Flutter extension.

## Install the Flutter SDK
- set up VS Code
- configure VS Code to point to your local Flutter SDK
- run the Flutter: New Web Project command from VS Code
- after the project is created, run your app by pressing F5 or "Debug -> Start Debugging"
- VS Code will use the webdev command-line tool to build and run your app; a new Chrome window should open, showing your running app

## Using from IntelliJ
- install the Flutter SDK
- set up your copy of IntelliJ or Android Studio
- configure IntelliJ or Android Studio to point to your local Flutter SDK
- create a new Dart project; note, for a Flutter for web app, you want to start from the Dart project wizard, not the Flutter project wizard
- from the Dart project wizard, select the 'Flutter for web' option for the application template
- create the project; pub get will be run automatically
- once the project is created, hit the run button on the main toolbar
- IntelliJ will use the webdev command-line tool to build and run your app; a new Chrome window should open, showing your running app

## Workflow for terminal
1. Install Dart Framework (for web demonstration)
[brew tap dart-lang/dart]
[brew install dart]
[pub global activate webdev]
[pub global activate stagehand]
::Add command to .zsh_profile - export PATH="$PATH":"$HOME/.pub-cache/bin”
[source ~/.zshrc]

2. Install Flutter Framework
[> mkdir ~/Library/Development && cp ~/Downloads/flutter_macos_v1.5.4-hotfix.2-stable.zip ~/Library/Development]
[> cd ~/Library/Development && unzip flutter_macos_v1.5.4-hotfix.2-stable.zip]
::Add command to .zsh_profile - export PATH="$PATH":"$HOME/Library/Development/flutter/bin"
[> source ~/.zshrc]
[> cd Projects]
[> mkdir DartProjects && cd DartProjects]
[> mkdir quickstart && cd quickstart]
[> pub global activate stagehand]
[> stagehand]
[> stagehand web-simple]
[> pub get]
[> webdev serve --auto restart]
::Run web project: http://localhost:8080/

3. Create Flutter Project
[> brew upgrade cocoapods]
[> sudo gem install cocoapods]
[> pod setup]
[> pod --version => must be 1.5.0 or greater]
[> cd DartProjects]
[> git clone https://github.com/ibhavikmakwana/FlutterPlayground.git FlutterPlayground]
[> cd FlutterPlayground]
[> flutter upgrade]
[> flutter precache]
[> flutter config --no-analytics]
[> flutter pub global activate webdev]
[> flutter packages pub global activate webdev]
[> flutter emulators => take emulatorID]
[> flutter emulators --launch apple_ios_simulator]
[> flutter run]
