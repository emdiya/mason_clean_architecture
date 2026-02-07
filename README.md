# Mason Clean Architecture (GetX)

A Mason brick template to scaffold a Flutter feature module using Clean Architecture and GetX.

## Prerequisites

- Flutter SDK installed
- Dart SDK installed
- Mason CLI installed

Install Mason CLI:

```bash
dart pub global activate mason_cli
```

Make sure Mason is in your PATH.

- macOS/Linux (`zsh`):

```bash
echo 'export PATH="$PATH:$HOME/.pub-cache/bin"' >> ~/.zshrc
source ~/.zshrc
```

- Windows (PowerShell): add this folder to your `Path` environment variable:

```text
C:\Users\<Your_Username>\AppData\Local\Pub\Cache\bin
```

Verify installation:

```bash
mason --version
```

## Use This Brick in Any Project

### 1) Create/open a Flutter project

```bash
flutter create my_new_project
cd my_new_project
```

### 2) Initialize Mason

```bash
mason init
```

### 3) Add this brick (run in your Flutter project root)

```bash
mason add features --git-url https://github.com/emdiya/mason_clean_architecture --git-path bricks/features
```

### 4) Generate a feature

```bash
mason make features
```

Example prompt:

```text
? What is your module name? (Main): home
```

Generated files will be created under:

```text
lib/features/<feature_name>/
```

## Install Globally (Optional)

If you want to use the brick across projects without re-adding each time:

```bash
mason add -g features --git-url https://github.com/emdiya/mason_clean_architecture.git --git-path bricks/features
```

Then in any project:

```bash
mason make features
```

## Update or Reinstall

```bash
mason remove -g features
mason add -g features --git-url https://github.com/emdiya/mason_clean_architecture.git --git-path bricks/features
```

## Local Development

This repository includes a `mason.yaml` configured for the `features` brick:

```yaml
bricks:
  features:
    git:
      url: "https://github.com/emdiya/mason_clean_architecture.git"
      path: bricks/features
```

You can run `mason get` to pull the configured brick.

## Author

Prepared by DiYA:

- GitHub: https://github.com/emdiya
- Medium: https://medium.com/@emdiya
