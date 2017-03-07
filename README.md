# prime-docs
Prime install process

There are three ways you can get started making a BoldGrid Child Theme.  You will first need the [Prime parent theme](https://github.com/boldgrid/prime).

## 1. Using the build tools supplied (preferred). ##

Go into the WordPress themes folder:

```shell
$ cd wp-content/themes
```


Clone the theme into your WordPress themes folder:

```shell
$ git clone https://github.com/boldgrid/prime
```

Now switch to the theme directory:

```shell
$ cd prime
```

In theme directory, you would run this command to install the npm dependencies:

```shell
$ npm install
```

Then you should run the task runner, which is the gulp process:

```shell
$ gulp install-framework
```

## 2. Clone the git repo and run the theme framework clone script. ##

Go into the WordPress themes folder:

```shell
$ cd wp-content/themes
```

Clone the theme into your WordPress themes folder:

```shell
$ git clone https://github.com/boldgrid/prime
```

Switch to the prime folder:

```shell
$ cd prime
```

Then run the clone script:

```shell
$ bash clone
```
## 3. Manual Installation. ##

You can download the Prime parent theme from the github repo: https://github.com/BoldGrid/prime/archive/master.zip
Unzip the file, into a folder in wp-content/themes.
Now download the BoldGrid Theme Framework from the github repo: https://github.com/BoldGrid/boldgrid-theme-framework/archive/master.zip
Unzip the file, and place the contents of the folder inside called boldgrid-theme-framework/ into wp-content/themes/prime.
