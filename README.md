xdeploy
============================
[![Build Status](https://img.shields.io/travis/17zuoye/xdeploy/master.svg?style=flat)](https://travis-ci.org/17zuoye/xdeploy)

Deploy changing dependent projects faster, such as batch processing
tasks, e.g. submit a Python script or a Hive script to YARN.


How does `xdeploy` deploy projects ?
----------------------------
1. Change your code in your serveral related projects.
2. `rsync` these projects to server, it's really fast, except for full sync in the first time.
3. Detect some changed codes, and re-install related projects.
4. Launch your project and debug ...

Benefits
----------------------------
1. Every command is print to console detailly, not a black box, RAW SHELL SCRIPT rocks!
2. To run this script, only Python and its standard library is needed, no need to install thirty-party libraries.
3. Create a `virtualenv` environment automatically.

Usage
----------------------------
```bash
wget https://raw.githubusercontent.com/17zuoye/xdeploy/master/xdeploy
chmod +x xdeploy
mv -f xdeploy /usr/local/bin/
xdeploy
```


TODO
----------------------------
1. I want a feature X ? ... please [create an issue](https://github.com/17zuoye/xdeploy/issues), or [fork it](https://github.com/17zuoye/xdeploy/).
