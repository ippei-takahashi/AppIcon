# AppIcon

![platforms](https://img.shields.io/badge/platforms-iOS-333333.svg)
[![GitHub license](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/Nonchalant/AppIcon/master/LICENSE.md)
[![GitHub release](https://img.shields.io/github/release/Nonchalant/AppIcon.svg)](https://github.com/Nonchalant/AppIcon/releases)
![Xcode](https://img.shields.io/badge/Xcode-8.3-brightgreen.svg)
![Swift](https://img.shields.io/badge/Swift-3.1-brightgreen.svg)
[![Swift Package Manager compatible](https://img.shields.io/badge/Swift%20Package%20Manager-compatible-brightgreen.svg)](https://github.com/apple/swift-package-manager)

`AppIcon` generates `*.appiconset` contains each resolution image for iOS.

```
AppIcon.appiconset
├── Contents.json
├── Icon-App-20.0x20.0@2x.png
├── Icon-App-20.0x20.0@3x.png
├── Icon-App-29.0x29.0@2x.png
├── Icon-App-29.0x29.0@3x.png
├── Icon-App-40.0x40.0@2x.png
├── Icon-App-40.0x40.0@3x.png
├── Icon-App-60.0x60.0@2x.png
└── Icon-App-60.0x60.0@3x.png
```

## Demo

![](Document/Images/appicon.gif)

## Installation

### Homebrew

```
$ brew install Nonchalant/appicon/appicon
```

### Manual

Clone the master branch of the repository, then run make install.

```
$ git clone https://github.com/Nonchalant/AppIcon.git
$ make install
```

## Usage

`AppIcon` needs base image(`.png`). The size of base image is 1024x1024 pixel preferably.

```
$ appicon iTunesIcon-1024x1024.png
```

## Option

You can see options by `appicon --help`.

#### --output

Default: `AppIcon`

## Develop

### Generate Xcode project

```
$ cd AppIcon
$ swift package generate-xcodeproj
```

or

```
$ cd AppIcon
$ make xcode
```

## Author

Takeshi Ihara <afrontier829@gmail.com>

## License

Appicon is available under the MIT license. See the LICENSE file for more info.
