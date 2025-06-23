# Color Detection Application

## Group Members

- Nikita Shakya  
  Roll No: 102317213  
  Contribution: Testing the App

- Kanwarajaybir Singh  
  Roll No: 102317223  
  Contribution: Code Implementation

- Advait Gautam  
  Roll No: 102317226  
  Contribution: Finding Suitable Dataset

---

## About the Project

This project presents a Color Detection Application built using Python and OpenCV. The application enables users to click anywhere on an image and instantly view the name and RGB values of the color at that pixel. By leveraging a color dataset and simple image processing techniques, the tool demonstrates practical applications in digital design, accessibility, and education.

---

## How It Works

- The user runs the application, which opens a window displaying the chosen image.
- When the user clicks anywhere on the image, the application detects the position of the click.
- The program retrieves the RGB values from the clicked pixel.
- It then searches through the color dataset (CSV file) to find the color name that most closely matches the selected pixel’s RGB values, using a simple distance calculation.
- The application displays a rectangle of the detected color along with its name, hex code, and RGB values on the image.
- The process can be repeated for any number of clicks, and the application updates the displayed information each time.
- The user can exit the application by pressing the 'Esc' key.

---

## Dataset

- The application uses a CSV file (`colors.csv`) containing color names, hexadecimal codes, and RGB values as the reference dataset.
- The pandas library is used to load and manipulate this data.

---

## Installation

1. Clone this repository to your local machine.
2. Ensure you have Python installed (preferably 3.7 or above).
3. Install the required libraries:
   - OpenCV
   - pandas
   - numpy

   You can install them using pip:
  
   "pip install opencv-python pandas numpy"


4. Place your image and `colors.csv` dataset in the appropriate directories as specified in the script.

---

## Usage

- Run the main Python script.
- An image window will open.
- Click anywhere on the image to detect the color at that pixel.
- The detected color name, hex code, and RGB values will be displayed on the image.
- Press 'Esc' to exit the application.

---

## Experimental Evaluation

The application was tested on diverse images, including natural scenes and synthetic color charts. It accurately identified standard colors present in the dataset and displayed the correct color name and RGB values. The interface was responsive, and the color overlay provided clear visual feedback. Limitations were observed for colors not present in the dataset or in cases of gradients and shadows.

---

## Results and Discussion

The color detection application effectively identifies and displays color information for user-selected pixels. Its accuracy depends on the comprehensiveness of the color dataset. The application is robust for standard colors but may mislabel colors not present in the CSV file. The real-time feedback and interactive interface make it suitable for educational and design purposes. Future improvements could include a larger dataset and more sophisticated color difference algorithms.

---

## Related Work

Other color detection projects using OpenCV often use HSV color space and masking techniques for color segmentation. This project focuses on direct pixel-based color matching and name identification using a CSV dataset, making it straightforward and educational.

---

## Future Work

- Expand the dataset to include a broader and more diverse set of color names.
- Enhance the algorithm using perceptual color difference metrics or machine learning for improved accuracy.
- Adapt the application for mobile or web platforms.
- Add accessibility features such as voice output or color-blind friendly modes.

---

## Conclusion

This Color Detection Application demonstrates how Python and OpenCV can be used to build interactive and educational computer vision tools. The project provides a foundation for further exploration in color analysis, image processing, and user interface design.

---
