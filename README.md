# GitHub Report

GitHub Report tool.

- Free software: BSD 3 Clause
- Documentation: https://opensciencelabs.github.io/ghreports

## Configuration file

In order to create a configuration file, add to your project, at the root level,
a file called .ghreports.yaml, with the following structure:

```yaml
name: myproject-name-slug
title: "My Report Title"
env-file: .env
repos:
  - myorg-1/myproject1
authors:
  - gh-username-1: GitHub Username 1
output-dir: "/tmp/ghreports"
```

## How to run the ghreports

```bash

ghreports --start-date 2025-07-01 --end-date 2025-07-31 --config-file tests/.ghreports.yaml

```

You can also specify the token in the command line as an argument:

```bash

ghreports --start-date 2025-07-01 --end-date 2025-07-31 --gh-token blabla --config-file tests/.ghreports.yaml

```
