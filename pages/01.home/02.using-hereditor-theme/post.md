---
title: "Using Hereditor theme"
slug: using-hereditor-theme
date: "03-03-2022 16:00"
taxonomy:
  tag:
    - settings
image: JazIGJ8_iw4.jpg
published: true
---

## Using the skeleton

The simplest way to install _Hereditor_ theme is to download and install the _Hereditor_ skeleton package:

1. Download [_Hereditor_ skeleton](https://github.com/gizmecano/grav-skeleton-hereditor-site)
2. Unzip the package into your web root folder.
3. Point your browser at the folder.

Check out the [general Grav installation instructions](https://learn.getgrav.org/basics/installation) for more details on this process.

It is possible to install just the theme as described below, but page content will need to fit the templates supported by _Hereditor_ theme. It is strongly advised to at least install the _Hereditor_ skeleton package as described above to see the structuration of the theme in action.

## Installing the theme

<!--Installing the _Hereditor_ theme can be done in one of two ways. Using the GPM (Grav Package Manager) installation method enables to quickly and easily install the theme with a simple terminal command, while the manual method enables to do so via a `zip` file.

### GPM installation

The simplest way to install the theme is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm) through the system's Terminal (also called _the command line_). From the root of the Grav install type:

```bash
bin/gpm install hereditor
```

This will install the _Hereditor_ theme into your `/user/themes` directory within Grav. Its files can be found under `/your/site/grav/user/themes/hereditor`.-->

### Manual installation

To install the theme, just download the `zip` version of this repository and unzip it under `/your/site/grav/user/themes`. Then, rename the folder to `hereditor`. These files can be found <!--either--> on [GitHub](https://github.com/gizmecano/grav-theme-hereditor/)<!-- or via [GetGrav.org](http://getgrav.org/downloads/themes)-->.

All the _Hereditor_ theme files should be into the folder `/your/site/grav/user/themes/hereditor`.

## Updating the theme

As development for the _Hereditor_ theme continues, new versions may become available that add additional features and functionality, improve compatibility with newer Grav releases, and generally provide a better user experience. <!--Updating _Hereditor_ is easy, and can be done through Grav's GPM system, as well as manually.-->

<!--### GPM update

The simplest way to update this theme is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm). Navigate to the root directory of the Grav install using the system's Terminal (also called _command line_) and type the following:

```bash
bin/gpm update hereditor
```

This command will check the Grav install to see if the _Hereditor_ theme is due for an update. If a newer release is found, it will be asked whether or not proceed to update. To continue, type `y` and hit enter. The theme will automatically update and clear Grav's cache.-->

### Manual update

Manually updating _Hereditor_ is pretty simple:

- Delete the `your/site/user/themes/hereditor` directory
- Download the new version of the _Hereditor_ theme from <!--either--> [GitHub](https://github.com/gizmecano/grav-theme-hereditor/)<!-- or [GetGrav.org](https://getgrav.org/downloads/themes)-->
- Unzip the `zip` file in `your/site/user/themes` and rename the resulting folder to `hereditor`
- Clear the Grav cache using admin panel or following command:

```bash
bin/grav clear-cache
```

Note that any changes made to any of the files listed under this directory will also be removed and replaced by the new set. Any files located elsewhere (for example a ``YAML`` settings file placed in `user/config/themes`) will remain intact.
