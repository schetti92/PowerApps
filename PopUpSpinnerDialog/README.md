# Fully Customizable Responsive Popup Spinner Component for Power Apps

## Overview

The COM_WaitTimer component is a fully customizable and responsive popup spinner for Power Apps. It works seamlessly across mobile, tablet, and desktop screens. This component allows you to display a loading indicator with a customizable spinner image and text while performing background operations.

![Intro](./localImages/COMVIEW.gif)

## Features

- Fully responsive design for mobile, tablet, and desktop
- Customizable spinner image (changeable via App formulas)
- Adjustable dialog width and height
- Custom wait text message
- Built-in visibility control
- Supports shadow and padding configurations

## Technology Stack

- **PowerApps**: The platform used to create the application and design the user interface.
---
## How to Use

- Import the COM_WaitTimer component into your Power Apps project.
- Place it in the required screen.
- Modify the properties using Power Apps formulas
   ```powerapps
    COM_WaitTimer.WaitText = "Loading... Please wait."
    COM_WaitTimer.spinnerImage = "[Your Spinner GIF URL]"
    COM_WaitTimer.DialogWidth = 300  // Adjust as needed
- Use the **DialogSetVisibility** action to control the popup:
   ```powerapps
    COM_WaitTimer.DialogSetVisibility(true) // Show the spinner
    COM_WaitTimer.DialogSetVisibility(false) // Hide the spinner

## Changing the Spinner Image

You can replace the default spinner GIF with a custom one by setting the `spinnerImage` property. You can create spinning GIFs using [loading.io](https://loading.io/).


### Screenshots



## Regards - Shashika Hettiarachchi ❤️
