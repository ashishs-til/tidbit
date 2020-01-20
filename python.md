# Python

**Removing (user-installed) Python from Mac-OS**
```
sudo rm -rf /Library/Frameworks/Python.framework/Versions/3.X
sudo rm -rf "/Applications/Python 3.X"
cd /usr/local/bin/
ls -l /usr/local/bin | grep '../Library/Frameworks/Python.framework/Versions/3.X' | awk '{print $9}' | tr -d @ | xargs rm
```
