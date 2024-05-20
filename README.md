## Overview

Overview
The **OpenTechSummit Website** is the official web platform for the OpenTechSummit, a premier technology summit showcasing the latest advancements in open technologies. This project houses the frontend components, including a customized version of Bootstrap to deliver a dynamic and responsive user experience.

##
Overview

This project forms the basis for the website of OpenTechSummit, featuring image optimization, custom scripts, and several plugin integrations for a smooth user experience. This README provides details on the installation, usage, and structure of the project.

##
## Features

Features

- **Image Optimization**: Optimization of images for faster load times using Gulp and imagemin.
- **Sticky Navigation**: Adds sticky navigation that remains at the top as the user scrolls down.
- **Smooth Scrolling**: Implements smooth scrolling for links.
- **Responsive Design Fixes**: Provides fixes for viewport scaling on iPhones.
- **Bootstrap Integration**: Uses Bootstrap for responsive UI elements.
- **Countdown Timer**: Includes a countdown timer plugin for events.
- **Lightbox**: Lightbox support for displaying images and galleries.
- **Instagram API Integration**: Fetches and displays Instagram posts.
- **Twitter API Integration**: Fetches and displays tweets.

##
Features
- Dynamic theming using custom Bootstrap JavaScript components.
- Comprehensive navigation including buttons, modals, dropdowns, and more.
- Interactive elements like carousels, tooltips, and collapsible sections.
- Event tracking with a scroll spy functionality.
- Flexible and reusable UI components.

##
## Installation Instructions

Installation Instructions

1. **Clone the Repository**

   ```sh
   git clone https://github.com/OpnTec/opentechsummit.de.git
   ```

2. **Navigate to the Project Directory**

   ```sh
   cd opentechsummit.de
   ```

3. **Install Node.js and npm** (if not already installed)

   Refer to the [Node.js website](https://nodejs.org/) for instructions.

4. **Install Gulp Globally**

   ```sh
   npm install --global gulp-cli
   ```

5. **Install Project Dependencies**

   ```sh
   npm install
   ```

6. **Run the Default Gulp Task**

   This will optimize the images in the `img` directory.

   ```sh
   gulp
   ```

##
Installation Instructions
To set up the project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/OpnTec/opentechsummit.de.git
   cd opentechsummit.de
   ```

2. **Install dependencies:**
   Ensure you have Node.js and npm installed. Run:
   ```bash
   npm install
   ```

3. **Build the project:**
   ```bash
   npm run build
   ```

4. **Start the development server:**
   ```bash
   npm start
   ```
   Open your web browser and navigate to `http://localhost:3000` to view the project.

##
## Usage Examples

Usage Examples

### Gulp Image Optimization

To optimize images, run the following Gulp command:

```sh
gulp images-opt
```

### Sticky Navigation

The sticky navigation is controlled by the script in `js/scripts.js`. It automatically adds a sticky class to the `nav` element when you scroll down.

```javascript
$(window).scroll(function() {
    if ($(window).scrollTop() > 1) {
        $('nav').addClass('sticky-nav');
    } else {
        $('nav').removeClass('sticky-nav');
    }
});
```

### Smooth Scrolling Implementation

This feature is enabled through jQuery plugin in `js/smooth-scroll.min.js`.

```javascript
// Usage
$('a').smoothScroll();
```

##
Usage Examples
Here are some examples of how to use the key components in the project:

### Button
```html
<button type="button" class="btn btn-primary">Primary Button</button>
```

### Modal
```html
<!-- Button to trigger modal -->
<button type="button" class="btn btn-info" data-toggle="modal" data-target="#myModal">Open Modal</button>

<!-- Modal Structure -->
<div id="myModal" class="modal fade" tabindex="-1" role="dialog">
  <div class="modal-dialog" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">Modal title</h5>
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
        <p>Modal body text goes here.</p>
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Save changes</button>
      </div>
    </div>
  </div>
</div>
```

### Tooltip
```html
<button type="button" class="btn btn-secondary" data-toggle="tooltip" data-placement="top" title="Tooltip on top">
  Tooltip on top
</button>
```

##
## Code Summary

Code Summary

### Key Files and Directories

- **gulpfile.js**: Contains Gulp tasks for image optimization.
- **javascripts/**: Directory containing custom JavaScript files:
  - `main.js`: Main JavaScript file that includes basic setup.
  - `scale.fix.js`: Viewport fixes for iPhone.
- **js/**: Directory with multiple JavaScript libraries and plugins:
  - `bootstrap.*.js`: Bootstrap JavaScript plugins.
  - `jquery.*.js`: Various jQuery plugins.
  - `scripts.js`: Custom scripts for navigation and other features.
- **variant/**: Contains variant requires JavaScript libraries and custom initializations.

##
Code Summary
The project structure includes the following key files:

- **`bootstrap.mix.js`**: Imports various Bootstrap JavaScript modules like transition, alert, button, carousel, collapse, dropdown, modal, tooltip, popover, scrollspy, tab, and affix.
- **`button.js`**: Contains JavaScript functionality for buttons.
- **`carousel.js`**: Implements carousel functionalities.
- **`collapse.js`**: Manages collapsible elements.
- **`dropdown.js`**: Handles dropdown menus.
- **`modal.js`**: Provides modal window functionalities.
- **`popover.js`**: Manages popovers.
- **`scrollspy.js`**: Facilitates scroll spy functionalities.
- **`tab.js`**: Handles tab navigation.
- **`tooltip.js`**: Manages tooltips.
- **`transition.js`**: Includes CSS transition support.

##
## License

License

This project is licensed under the MIT License. See the [LICENSE file](https://github.com/OpnTec/opentechsummit.de/blob/master/LICENSE) for details.
License
This project is licensed under the MIT License. See the [MIT License](https://github.com/twbs/bootstrap/blob/master/LICENSE) for more information.