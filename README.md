## Mason Template with Clean Architecture

`Noted:` Make sure you have Dart & Mason installed in your machine

```terminal
    dart pub global activate mason_cli
```

1: Install brick globally on machine :

```terminal
    mason add -g features --git-url https://github.com/emdiya/mason_clean_architecture --git-path bricks/features
```

2: How to use :

```terminal
    mason make feature
```

Note*: How to reinstall :

```terminal
   mason remove -g features
   mason add -g feature --git-url https://github.com/emdiya/mason_clean_architecture --git-path bricks/features
```

Enter your feature name

```terminal
    ? What is your module name? (Main) examplefeatures
```
