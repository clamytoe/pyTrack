# pyTrack
> Simple project/task time tracker for Python 3.6.0+.

[![GitHub issues][issues-image]][issues-url]
[![GitHub forks][fork-image]][fork-url]
[![GitHub Stars][stars-image]][stars-url]
[![License][license-image]][license-url]
[![Twitter][twitter-image]][twitter-url]

Helps you keep track of how much time you spend on your projects and tasks. A sqlite database is used to track your time logs, and it is kept simply by only implementing as few commands as needed to get a full featured application. You can add/remove multiple projects, start/stop tracking any of them, or completely reset the database to start with a clean slate.

## Installation

OS X & Linux:

```bash
cd
mkdir Projects
cd Projects
git clone https://github.com/clamytoe/pyTrack.git
python3.6 -m venv venv
source ./venv/bin/activate
pip install -r requirements.txt
python setup.py install
```

## Usage example

This application is really simple to use. To get help on the different commands simply add --help to the end of the command.

```bash
pytrack --help
Usage: pytrack [OPTIONS] COMMAND [ARGS]...

Options:
  --help  Show this message and exit.

Commands:
  add     Add a new project
  remove  Remove the project by the entered ID
  reset   Reset the database
  select  Marks the given project ID as selected
  start   Starts active tracking of project
  stop    Stops active tracking of project
```

## Development setup

If you would like to install this in order to play around with the code and make modifications yourself, simply change the last command in the installation instructions above to the following:

```bash
python setup.py develop
```

## Release History

* 0.2.1
    * CHANGE: Update docs (module code remains unchanged)
* 0.0.4
    * CHANGE: Refactored into a package
    * ADD: Added setup.py, README.md, LICENSE
* 0.0.3
    * ADD: Added PeeWee backend and started using Maya for datetime objects
* 0.0.2
    * The first true commandline version
    * CHANGE: Modified into a commandline utility
    * ADD: Started using click
* 0.0.1
    * Work in progress

## Meta

Martin Uribe – [@mohhinder](https://twitter.com/mohhinder) – clamytoe@gmail.com

Distributed under the MIT license. See ``LICENSE`` for more information.

[https://github.com/clamytoe/pyTrack](https://github.com/clamytoe/)

[issues-image]:https://img.shields.io/github/issues/clamytoe/pyTrack.svg
[issues-url]:https://github.com/clamytoe/pyTrack/issues
[fork-image]:https://img.shields.io/github/forks/clamytoe/pyTrack.svg
[fork-url]:https://github.com/clamytoe/pyTrack/network
[stars-image]:https://img.shields.io/github/stars/clamytoe/pyTrack.svg
[stars-url]:https://github.com/clamytoe/pyTrack/stargazers
[license-image]:https://img.shields.io/badge/license-MIT-blue.svg
[license-url]:https://raw.githubusercontent.com/clamytoe/pyTrack/master/LICENSE
[twitter-image]:https://img.shields.io/twitter/url/https/github.com/clamytoe/pyTrack.svg?style=social
[twitter-url]:https://twitter.com/intent/tweet?text=Wow:&url=%5Bobject%20Object%5D
