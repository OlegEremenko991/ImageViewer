
[![CI Status](http://img.shields.io/travis/Krisiacik/ImageViewer.svg?style=flat)](https://travis-ci.org/Krisiacik/ImageViewer)
[![Swift 5.0](https://img.shields.io/badge/Swift-5.0-green.svg?style=flat)](https://developer.apple.com/swift/)
[![Version](https://img.shields.io/badge/SPM-supported-DE5C43.svg?style=flat)](https://swift.org/package-manager/)
[![Platforms iOS](https://img.shields.io/badge/Platforms-iOS-lightgray.svg?style=flat)](https://developer.apple.com/swift/)
[![License MIT](https://img.shields.io/badge/License-MIT-lightgrey.svg?style=flat)](https://opensource.org/licenses/MIT)

![Single image view](https://github.com/Krisiacik/ImageViewer/blob/master/Documentation/single.gif)

![Gallery](https://github.com/Krisiacik/ImageViewer/blob/master/Documentation/gallery.gif)

For the latest changes see the [CHANGELOG](CHANGELOG.md)

## Install

### Swiftpackage

Just add the repository URL in Xcode

## Sample Usage

For a detailed example, see the [Example](https://github.com/OlegEremenko991/ImageViewer/tree/main/Example)

```swift
// Show the ImageViewer with the first item
self.presentImageGallery(GalleryViewController(startIndex: 0, itemsDataSource: self))

// The GalleryItemsDataSource provides the items to show
extension ViewController: GalleryItemsDataSource {
    func itemCount() -> Int {
        return items.count
    }

    func provideGalleryItem(_ index: Int) -> GalleryItem {
        return items[index].galleryItem
    }
}

```

### ImageViewer version vs Swift version.

ImageViewer 6.0 is Swift 5 ready

## License

ImageViewer is licensed under the MIT License, Version 2.0. See the [LICENSE](LICENSE) file for more info.

Copyright (c) 2016 MailOnline
