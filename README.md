## Mason Template with Clean Architecture Getx Statemanagement

`Noted:` Make sure you have Dart & Mason installed in your machine
Open terminal

```base
    dart pub global activate mason_cli
```

## Window Configuration

1: Install brick globally on machine :

#### Clone Project into local machine

```
git clone https://github.com/emdiya/mason_clean_architecture C:/Users/DiYA/AppData/Local/Mason/Cache/git/mason_clean_architecture

```

#### Add Mason features

```terminal
    mason add -g features --git-url https://github.com/emdiya/mason_clean_architecture --git-path bricks/features
```

If you see ✓ Added features it`s mean you have been add successully

# How to install in new project ?

Create a New Dart Project

```
dart create my_new_project
cd my_new_project
```

Activate Mason CLI:

```
dart pub global activate mason_cli
```

Add Mason to Your Project:
Add Mason as a dependency in your pubspec.yaml file. Open pubspec.yaml and add:

```
dependencies:
  mason: anyversion
```

Install Dependencies:

```
dart pub get
```

Initialize Mason: Initialize Mason in your project directory:

```
mason init
```

Add Bricks: Add the desired brick (in your case, "features") to your Mason configuration. Here is how you can add a brick from a Git repository:

```
mason add features --git-url https://github.com/emdiya/mason_clean_architecture --git-path bricks/features
```

2: How to use :
Generate Features: Once the brick is added, you can generate the features:

```terminal
    mason make features
```

Enter your feature name

```terminal
    ? What is your module name? (Main): home
```

`Noted:` How to reinstall :

```terminal
   mason remove -g features
   mason add -g feature --git-url https://github.com/emdiya/mason_clean_architecture --git-path bricks/features
```
