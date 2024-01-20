
# Image Viewer App

## Description
This iOS application utilizes the Unsplash API to fetch stunning images and displays them using the powerful URLSession in Swift. The app also incorporates the SDWebImage pod for efficient image loading and caching. With a user-friendly interface, the app provides features such as an image carousel, a scrollable list with search functionality, offline capability, and the ability to view label details on a separate screen.

## Features

### 1. Image Carousel

- Swipe left or right to navigate through a seamless image carousel.
- Dynamically adjusts to handle any number of images.

### 2. Scrollable List

- Scroll up or down to explore a list of images.
- Capable of handling any number of items efficiently.

### 3. Search Functionality

- Utilize the search bar to filter labels in the list based on user input.
- Search bar pins to the top for convenient access.

### 4. Offline Capability

- Cache data locally for offline access when an internet connection is not available.

### 5. Label Details

- Click on a label to view detailed information on a separate screen.





## Getting Started

These instructions will help you get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Make sure you have the following installed on your development machine:

- [Xcode](https://developer.apple.com/xcode/)
- [CocoaPods](https://cocoapods.org/)

 
### Installation

Follow these steps to set up and run the project:

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/your-username/your-project.git
   ```

2. Navigate to the project directory:

   ```bash
   cd your-project
   ```

3. Open the `Podfile` in the root directory and add the following lines to include `SDWebImage`:

   ```ruby
   # Podfile

   platform :ios, '11.0'
   use_frameworks!

   target 'ImageDemo' do
     # Add other pods if needed

     # Include SDWebImage
     pod 'SDWebImage', '~> 5.0'
   end
   ```

4. Save the `Podfile` and close it.

5. Install project dependencies using CocoaPods:

   ```bash
   pod install
   ```

   This will install the required dependencies, including `SDWebImage`.

6. Open the Xcode workspace (`.xcworkspace`) file:

   ```bash
   open ImageDemo.xcworkspace
   ```

7. Build and run the project from Xcode.

 ## Dependencies

- [Unsplash API](https://unsplash.com/developers) - Open API for fetching beautiful images.
- [SDWebImage](https://github.com/SDWebImage/SDWebImage) - Third-party pod for efficient image loading and caching.
  
### Usage

Explain how users can interact with your project. Provide code snippets or examples for common use cases.

```swift
import SDWebImage

// Example usage of SDWebImage
imageView.sd_setImage(with: URL(string: "https://example.com/image.jpg"), placeholderImage: UIImage(named: "placeholder"))
```









## Demo Videos and Images
| Showcase of Image Carousel and List Scroll                       |   Search Functionality in Action                      |
| ----------------------------------- | ----------------------------------- |
| ![Demo Video 1](https://github.com/rohit-dseu/1/blob/main/WhatsApp%20Video%202024-01-20%20at%2011.50.24%20PM.gif) | ![Demo Video 2](https://github.com/rohit-dseu/1/blob/main/WhatsApp%20Video%202024-01-20%20at%2011.49.47%20PM.gif)|





# Project Structure

## View
- *MainViewController.swift:* Main view controller orchestrating the application's primary functionality.
- *ViewController.swift:* Generic view controller handling UI and user interactions.
- *ImagesCell.swift:* Swift file defining a custom cell for displaying images in a table or collection view.
- *ImagesCell.xib:* Interface Builder file associated with the ImagesCell.swift for designing the custom image cell.
- *ListTableViewCell.swift:* Swift file for a table view cell used in a list-based display.
- *ListTableViewCell.xib:* Interface Builder file associated with the ListTableViewCell.swift for designing the custom list table view cell.
- *ImagesCarouselCell.swift:* Swift file defining a custom cell for an image carousel or slider.
- *ImagesCarouselCell.xib:* Interface Builder file associated with the ImagesCarouselCell.swift for designing the custom image carousel cell.

## ViewModel
- *YourViewModel.swift:* ViewModel managing the interaction between the View and Model.
- *Product+CoreDataProperties.swift:* CoreData-generated Swift file with additional properties for the "Product" entity.
- *Product+CoreDataClass.swift:* CoreData-generated Swift file representing the "Product" entity as a class.
- *ImageModel.swift:* Swift file defining a model for handling image-related data or functionality.

## Model
- *YourModel.swift:* Model representing the data and business logic of the application.

## Other Folders and Files
- Additional folders and files as needed.

## Supporting Files
- Supporting files like AppDelegate, Info.plist, etc.
