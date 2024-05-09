# Automating Redundant Work on Shiprocket with Python AutoGUI

## Overview

This project aims to automate redundant tasks performed on the Shiprocket website, specifically targeting operations tasks encountered by Dotstore, a startup. By leveraging the Python AutoGUI library, this script streamlines processes such as checking product dimensions, verifying delivery partners, and other repetitive actions. This README provides an overview of the project structure, setup instructions, and usage guidelines.

## Features

- **Product Dimension Check**: Automatically verifies the dimensions of products listed on Shiprocket.
- **Delivery Partner Evaluation**: Automates the process of checking and evaluating delivery partners.
- **Customizable and Extensible**: Script can be easily modified to accommodate additional tasks and functionalities.

## Requirements

- Python 3.x
- Python AutoGUI library
- Web browser with access to the Shiprocket website

## Installation

1. Clone or download this repository to your local machine.
2. Install Python if not already installed.
3. Install the required Python libraries by running:
   ```
   pip install pyautogui
   ```

## Usage

1. Open your preferred web browser and navigate to the Shiprocket website.
2. Ensure that you are logged in to your account.
3. Run the Python script `shiprocket_automation.py`.
4. Follow any on-screen prompts or instructions provided by the script.

## Customization

- **Coordinates Configuration**: Adjust the coordinates used for mouse clicks and interactions based on the layout of the Shiprocket website. Update the coordinates in the script to match the locations of buttons, fields, and other elements.
- **Error Handling**: Implement additional error handling and exception management to ensure robustness and reliability of the automation process.
- **Additional Tasks**: Extend the script to automate other tasks and workflows as needed for your specific requirements.

## Example

```python
import pyautogui
import time

# Wait for the user to open the browser and navigate to the Shiprocket website
time.sleep(5)

# Click on the product dimensions section and retrieve information
pyautogui.click(100, 200)  # Example coordinates, replace with actual coordinates
product_dimensions = pyautogui.locateOnScreen('product_dimensions.png')  # Example image recognition, replace with actual method

# Click on the delivery partners section and evaluate options
pyautogui.click(100, 250)  # Example coordinates, replace with actual coordinates
delivery_partners = pyautogui.locateOnScreen('delivery_partners.png')  # Example image recognition, replace with actual method
```

## Disclaimer

This script is provided as-is and may require customization to suit individual requirements. Use with caution and ensure compliance with all terms of service and usage policies of the Shiprocket platform.
