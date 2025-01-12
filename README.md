# License Plate Detection Project

This project implements a license plate detection and annotation system using OpenCV. It processes vehicle images and adds a green rectangle around the license plate area along with the license plate number overlay.

## Features

- License plate area detection and highlighting
- License plate number overlay with semi-transparent background
- Configurable annotation parameters
- Image saving functionality

## Requirements

- Python 3.x
- OpenCV (opencv-python==4.10.0.84)
- NumPy (numpy==2.2.1)

## Installation

1. Clone this repository
2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

The main script `app.py` contains the license plate annotation functionality. To use it:

1. Place your input image in the `images` folder
2. Run the script:
   ```bash
   python app.py
   ```

The script will:
- Load the input image from `./images/assignment-001-given.jpg`
- Add a green rectangle around the detected license plate area
- Add the license plate number (RAH972U) with a semi-transparent background
- Save the result as `result.jpg` in the images folder
- Display the processed image

## Project Structure

```
├── app.py              # Main application file
├── images/             # Directory for input and output images
├── requirements.txt    # Project dependencies
└── README.md          # Project documentation
```

## License Plate Annotation Details

The script performs the following operations:
- Draws a green rectangle around the license plate area
- Adds the license plate number in the top-right corner
- Creates a semi-transparent background for the text
- Saves the annotated image

## Error Handling

The script includes error handling for:
- Image loading failures
- Processing errors
- File saving issues
