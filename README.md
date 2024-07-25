# Color-Detection-Application
This application detects the color name of any pixel in an image by clicking on it. It uses OpenCV for image processing and pandas to read the color data from a CSV file.


# Requirements
- **Python 3.x**
- **OpenCV**
- **pandas**
- **numpy**

# Installation

- Clone the repository or download the color_detection.py script and colors.csv file.

- Install the required Python libraries:

```bash
  pip install opencv-python pandas numpy 
```
- Ensure that color_detection.py and colors.csv are in the same directory.

# Usage
To run the script, use the following command in your terminal or command prompt:
```bash

python color_detection.py -i path/to/your/image.jpg 
```

Replace path/to/your/image.jpg with the actual path to the image file you want to use.

# How It Works
- **Load Image:** The script loads the image specified in the command line argument. If the image cannot be loaded, it prints an error message and exits.

- **Mouse Click Event:** The script waits for a left mouse click event on the image window. When a click is detected, it captures the x and y coordinates of the click.

- **Color Detection:** Using the RGB values of the clicked pixel, the script calculates the closest matching color name from the colors.csv file.

- **Display Color:** The script draws a rectangle and displays the color name along with its RGB values on the image. The text color is adjusted for readability based on the background color.

- **Exit:** Press the esc key to exit the application.

# Files

- color_detection.py: The main script for the color detection application.
- colors.csv: A CSV file containing color names and their corresponding RGB values.

# Example
```bash
python color_detection.py -i sample.jpg
```
This command will open the image sample.jpg. Click anywhere on the image to see the color name and its RGB values displayed on the image.

# Note
- For very light colors, the text will be displayed in black to ensure readability.
- The colors.csv file must be in the same directory as the script or provide the correct path to it within the script.

# Contributing
If you find any issues or have suggestions for improvements, feel free to create a pull request or open an issue in the repository.
