---
title: "Configuring the theme"
slug: configure-theme
date: "03-03-2022 16:30"
taxonomy:
  tag:
    - images
    - links
    - settings
image: upGZ5p92SHU.jpg
published: true
---

## Setup

### Theme activation

To set _Hereditor_ theme as the default theme, the steps to follow are:

- Navigate to `/your/site/grav/user/config`
- Open the `system.yaml` file
- Change the `theme:` setting to `theme: hereditor`
- Save the changes
- Clear the Grav cache using admin panel or following command:

```bash
bin/grav clear-cache
```

Once this is done, the new theme should be available on the frontend. Keep in mind any customizations made to the previous theme will not be reflected as all of the theme and templating information is now being pulled from the `hereditor` folder.

### Site parameters

In case _Hereditor_ theme is activated on a fresh Grav install, some parameters in the `user/config/site.yaml` file have to be populated:

1. `title`: name of your site
2. `description`: description of your site
3. `author.name`: name site owner
4. `author.email`: mail address of the site owner
5. `author.bio`: short one sentence biography

The file should look a bit like this:

```yaml
title: Website name
description: A short description for the purpose of the website
author:
  name: Author Name
  email: username@domain.tdl
  bio: A short description of the author of the website
```

### Custom styles for plugins

The _Hereditor_ theme includes custom styles for specific plugins ([Markdown Notices](https://github.com/getgrav/grav-plugin-markdown-notices), [Pagination](https://github.com/getgrav/grav-plugin-pagination)). To be properly loaded, the _Use built in CSS_ option has to be set to `false` (using the admin panel or configuring the `YAML` file in the `users/config/plugins/` folder):

```yaml
built_in_css: false
```

## Configuring images and links

### Website images

Basically, the _Hereditor_ theme is arranged to use two images for the entire website:

1. `logo`: used into default page and to link toward the home page (but also as basic shortcut icon). This image aims to represent the website and should not exceed a size close to 300px × 300px.
2. `author.image`: set as illustration in the mini-bio. This image aims to represent the author of an article and should not exceed a size close to 300px × 300px.

These two images have to be defined in your `/your/site/grav/user/config/site.yaml` file, such as:

```yaml
logo: /user/images/logo.png
author:
  image: /user/images/avatar.png
```

### Article header images

Header images can be used in articles which are based on the **post** template. Any header image has to be declared in the front-matter section of the post, by adding a tag `image` populated with a proper URL to the intented file, such as this code sample (if the image is set in the same folder as the article):

```yaml
image: header-image.jpg
```

### Social links

In order to set social profiles features to be embedded in _Hereditor_ theme configuration, add the following to your `/your/site/grav/user/config/site.yaml` file:

1. `social.icon`: name of the social platform
2. `social.link`: the main URL of the plateform
3. `social.user`: the specific user name on the plateform

Below is an example for a Twitter account:

```yaml
social:
  - icon: twitter
    link: https://twitter.com/
    user: username
```
