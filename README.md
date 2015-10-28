# LicensingVC

![Version](https://img.shields.io/github/tag/tiagomnh/LicensingViewController.svg)
![Swift](https://img.shields.io/badge/Swift-2.1-orange.svg)
![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)
![GitHub license](https://img.shields.io/badge/license-MIT-lightgrey.svg)

LicensingVC is a `UIViewController` subclass with a simple API for displaying licensing information.

Written in Swift 2.1.

## Usage

```swift
import LicensingViewController

let licensingViewController = LicensingViewController()

licensingViewController.title = "Acknowledgments"

let alamofireItem = LicensingItem(
    title: "Alamofire",
    license: License.MIT(owner: "Alamofire Software Foundation (http://alamofire.org/)", years: "2014")
)

let caniveteItem = LicensingItem(
    title: "Canivete",
    license: License.MIT(owner: "Tiago Henriques (http://tiagomnh.com)", years: "2015")
)

let kingfisherItem = LicensingItem(
    title: "Kingfisher",
    license: License.MIT(owner: "Wei Wang", years: "2015")
)

licensingViewController.items = [alamofireItem, caniveteItem, kingfisherItem]
```

### Screenshot

![Screenshot](https://raw.githubusercontent.com/tiagomnh/LicensingViewController/master/Screenshots/Screenshot1.png?token=ABA_gA2OP8REPotmSu05yO604Sb8G-Ljks5VsBOgwA%3D%3D)

## Requirements

- iOS 8.0+
- Xcode 7.1 (Swift 2.1)

## Installation

LicensingVC is available through [Carthage](https://github.com/Carthage/Carthage). To install
it, simply add the following line to your Cartfile:

```ruby
github "eeschimosu/LicensingViewController"
```

Then run `carthage update`.


## License

LicensingVC is available under the MIT license. See the LICENSE file for more info.
