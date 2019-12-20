---
title: "Home"
---
{%-include github.html -%}
# [ {{ site_project_title }} ]({{ site_repository_url }}) [![Build Status]](https://travis-ci.com/{{ site_owner_name }}/{{ site_project_title }})

## Usage

Once the [repository] is set and packages were deployed,
add it as source in your system `/etc/pacman.conf`:

```bash
[{{ site_project_title }}]
SigLevel = Optional TrustAll
Server = https://github.com/{{ site_owner_name }}/$repo/releases/download/$arch
```

From now on you are ready to install / update / remove / list packages in it:

```bash
# Update the system:
pacman -Syu

# List packages in repository:
pacman -Sl {{ site_project_title }}

# Install a package:
pacman -S <package_name>
```

## Contributions

If you want to contribute back some new feature you need to:

- Switch to `master` from your personal repository: `git checkout master && git pull`
- Create a new feature branch: `git checkout -b my-feature`
- Add and commit your changes
- Push on your remote branch and go to the suggested GitHub page to create a
  new pull request.

[Build Status]: https://travis-ci.com/{{ site_owner_name }}/{{ site_project_title }}.svg?branch=master
[repository]:   {{ site_repository_url }}/releases/
