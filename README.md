
# Electrum ADA - Lightweight Cardano Wallet

[![License](https://img.shields.io/badge/License-GNU%20GPL%20v3-blue.svg)](https://github.com/jokeradms/Electrum-ADA/blob/master/LICENCE)
[![Release](https://img.shields.io/github/release/jokeradms/Electrum-ADA.svg)](https://github.com/jokeradms/Electrum-ADA/releases/tag/v3.7.1)
[![Tag](https://img.shields.io/github/tag/jokeradms/Electrum-ADA.svg)](https://github.com/jokeradms/Electrum-ADA/releases/tag/v3.7.1)
![Open Source](https://img.shields.io/badge/Open%20Source-Yes-blue.svg)


Electrum ADA is a lightweight, secure wallet for Cardano (ADA), built with Python. It is an open-source project designed to be efficient and easy to use. The wallet uses Electrum's framework and focuses on simplicity while providing powerful features.

---

## Download


### Latest version: [v3.7.1](https://github.com/jokeradms/Electrum-ADA/releases/tag/v3.7.1)

We support Windows, macOS, and Linux.  
Select your preferred platform below to download the corresponding installer.

| Operating System | Download Link                                                                                                      |
|:----------------:|:-------------------------------------------------------------------------------------------------------------------:|
| **Windows** <br> <sub>Windows 10 or later</sub> | [![Download for Windows](https://img.shields.io/badge/Download-Windows-blue?logo=windows)](https://github.com/jokeradms/Electrum-ADA/releases/tag/v3.7.1) |
| **macOS** <br> <sub>macOS 10.14 or later</sub>   | [![Download for macOS](https://img.shields.io/badge/Download-macOS-blue?logo=apple)](https://github.com/jokeradms/Electrum-ADA/releases/tag/v3.7.1)       |
| **Linux** <br> <sub>Most modern distributions</sub> | [![Download for Linux](https://img.shields.io/badge/Download-Linux-blue?logo=linux)](https://github.com/jokeradms/Electrum-ADA/releases/tag/v3.7.1)       |


---

## 1. GETTING STARTED

To run Electrum from this directory, just do:

```bash
./electrum-ada
```

If you install Electrum on your system, you can run it from any directory:

```bash
sudo python setup.py install
electrum-ada
```

---

## 2. HOW OFFICIAL PACKAGES ARE CREATED

To build the official packages for Electrum ADA, run the following commands:

```bash
python mki18n.py
pyrcc4 icons.qrc -o gui/qt/icons_rc.py
python setup.py sdist --format=zip,gztar
```

For **Mac OS X**:

```bash
# On port-based installs
sudo python setup-release.py py2app

# On brew installs
ARCHFLAGS="-arch i386 -arch x86_64" sudo python setup-release.py py2app --includes sip

# Create the DMG package
sudo hdiutil create -fs HFS+ -volname "Electrum-ADA" -srcfolder dist/Electrum-ADA.app dist/electrum-ada-VERSION-macosx.dmg
```

---

## 3. CONTRIBUTING

We welcome contributions! Please feel free to submit pull requests, report issues, and suggest improvements.

For more information, please refer to our [Contributing Guidelines](https://github.com/jokeradms/Electrum-ADA/blob/master/CONTRIBUTING.md).

---

## 4. LICENSE

Electrum ADA is licensed under the [GNU GPL v3](https://github.com/jokeradms/Electrum-ADA/blob/master/LICENCE).

---

For more details, visit our [GitHub repository](https://github.com/jokeradms/Electrum-ADA).

Thank you for using Electrum ADA!
