
# Awesome Image Viewer App

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

## Solution/Assumptions

### Data Source

- The app fetches images from the Unsplash API. Ensure a stable internet connection for the initial data retrieval.
- Data is stored locally using a caching mechanism for offline access.

### Image Carousel

swift
// Swift code for handling image carousel
// Example code here


- The image carousel dynamically loads images from the Unsplash API, providing a smooth and interactive user experience.

### Scrollable List

swift
// Swift code for handling scrollable list
// Example code here


- The scrollable list contains labels associated with the fetched images.
- The list seamlessly scrolls with the entire page, allowing users to explore a vast collection of images.

### Search Functionality

swift
// Swift code for implementing search functionality
// Example code here


- The search bar enables users to filter labels in real-time, enhancing the overall user experience.
- The search bar is fixed at the top of the list for easy access and visibility.

### Offline Capability

swift
// Swift code for implementing offline capability
// Example code here


- Cached data allows users to access previously fetched images even without an internet connection.
- The app checks for cached data on startup and updates the cache when an internet connection is available.

### Label Details

swift
// Swift code for displaying label details
// Example code here


- Tapping on a label navigates the user to a separate screen displaying additional details about the selected label.

## Demo Videos and Images
| Showcase of Image Carousel and List Scroll                       |   Search Functionality in Action                      |
| ----------------------------------- | ----------------------------------- |
| ![Demo Video 1](https://github.com/rohit-dseu/1/blob/main/WhatsApp%20Video%202024-01-20%20at%2011.49.47%20PM.gif) | ![Demo Video 2](https://github.com/rohit-dseu/1/blob/main/WhatsApp%20Video%202024-01-20%20at%2011.49.47%20PM.gif)|

![Screenshot 1](screenshot_1.png) - Image Carousel in Action

![Screenshot 2](screenshot_2.png) - Scrollable List with Search Bar

## Usage

To use the Awesome Image Viewer App, follow these steps:

1. **Clone the repository** to your local machine.
    bash
    git clone https://github.com/your-username/awesome-image-viewer.git
    

2. **Navigate to the project directory**.
    bash
    cd awesome-image-viewer
    

3. **Install Dependencies**. Ensure you have CocoaPods installed on your machine.
    bash
    pod install
    

4. **Open the Xcode project**. Open the generated `.xcworkspace` file to work with the project.

5. **Build and Run the app** on your iOS device or simulator.

## Dependencies

- [Unsplash API](https://unsplash.com/developers) - Open API for fetching beautiful images.
- [SDWebImage](https://github.com/SDWebImage/SDWebImage) - Third-party pod for efficient image loading and caching.

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
