## Mason Template with Clean Architecture Getx Statemanagement

`Noted:` Make sure you have Dart & Mason installed in your machine
Open terminal

```base
    dart pub global activate mason_cli
```

Add Mason CLI to Environment Variables:

1. **Add Mason CLI to Environment Variables**:

    - Open the Start Menu and search for "Environment Variables."
    - Select "Edit the system environment variables."
    - Click on the "Environment Variables" button.
    - Under "System variables," find the `Path` variable and click "Edit."
    - Click "New" and add the path to the directory where Dart and Mason CLI are installed, typically:

      ```plaintext
      C:\Users\<Your_Username>\AppData\Local\Pub\Cache\bin
      ```

    - Click "OK" to close all dialog boxes.

2. **Verify Installation**:

    Open a new terminal and run:

    ```bash
    mason
    ```

    This should show the Mason CLI help if it’s correctly configured.

### macOS and Linux

1. **Add Mason CLI to Environment Variables**:

    Open your terminal and run:

    ```bash
    echo 'export PATH="$PATH":"$HOME/.pub-cache/bin"' >> ~/.bashrc
    source ~/.bashrc
    ```

    If you are using `zsh`, replace `~/.bashrc` with `~/.zshrc`.

2. **Verify Installation**:

    Run the following command in your terminal:

    ```bash
    mason
    ```

    This should display the Mason CLI help if it’s set up correctly.

1: Install brick globally on machine :

#### Clone the Project on window

Open Terminal

```bash
git clone https://github.com/emdiya/mason_clean_architecture C:/Users/<Your_Username>/AppData/Local/Mason/Cache/git/mason_clean_architecture
```

> Note: Make sure to replace YOUR_USERNAME machine with your actual username.

---

### Clone the Project on macOS

Open your terminal and run:

```bash
git clone https://github.com/emdiya/mason_clean_architecture ~/Library/Mason/Cache/git/mason_clean_architecture
```

This command clones the repository to the specified directory in your local machine.

---

#### Add Mason features

Add Mason into machine follow bellow command:

```terminal
    mason add -g features --git-url https://github.com/emdiya/mason_clean_architecture --git-path bricks/features
```

> "If you see ✓ Added features, it means you have successfully added them.

# How to install in new project ?

Create a New Flutter Project

```
flutter create my_new_project
cd my_new_project
```

Activate Mason CLI:

```
dart pub global activate mason_cli
```

Add Mason to Your Project:
>Add Mason as a dependency in your pubspec.yaml file. Open pubspec.yaml and add:

```
dependencies:
  mason: ^0.1.0
```

Check lastest version in [pub.dev](https://pub.dev/packages/mason)

Install Dependencies:

```
flutter pub get
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

Here’s a more polished and standard version:

---

**Prepared by DiYA**  
For more, visit [DiYA on GitHub](https://github.com/emdiya) or follow [DiYA on Medium](https://medium.com/@emdiya).

---
