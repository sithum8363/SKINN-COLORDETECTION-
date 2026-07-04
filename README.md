# Skin Color Detection

A computer vision project for detecting and analyzing skin-colored regions in images or video frames. The project is intended as an educational demonstration of image processing, color-space analysis, segmentation, and basic computer vision techniques.

## Overview

Skin color detection is a common introductory computer vision task. A typical workflow converts an input image or camera frame into a suitable color space, applies threshold-based segmentation, cleans the resulting mask, and highlights the detected regions.

This repository can be used as a starting point for experiments involving:

- Image processing
- Color detection
- Skin-region segmentation
- Computer vision
- Real-time camera processing

## Features

- Processes image or video input
- Detects candidate skin-colored regions
- Uses color-based segmentation techniques
- Produces a mask for detected regions
- Can be extended for real-time webcam processing
- Suitable for learning basic computer vision workflows

## Technologies

Typical dependencies for this kind of Python computer vision project include:

- Python
- OpenCV
- NumPy

## Installation

Clone the repository:

```bash
git clone https://github.com/sithum8363/SKINN-COLORDETECTION-.git
cd SKINN-COLORDETECTION-
```

Create and activate a virtual environment if desired, then install the dependencies used by the source code.

For an OpenCV and NumPy implementation:

```bash
pip install opencv-python numpy
```

## Running the Project

Run the project's main Python script:

```bash
python main.py
```

If the repository uses a different entry-point filename, replace `main.py` with the actual source filename.

## General Processing Workflow

A color-detection pipeline commonly follows these steps:

1. Read an image or capture a frame from a camera.
2. Convert the image into the color space used by the detector.
3. Apply lower and upper color thresholds.
4. Generate a binary mask.
5. Apply optional noise-reduction operations.
6. Extract or highlight detected regions.
7. Display or save the result.

## Example Project Structure

```text
SKINN-COLORDETECTION-/
├── main.py
├── requirements.txt
├── LICENSE
└── README.md
```

The actual repository structure may differ depending on the source files in the project.

## Limitations

Color-based skin detection has important technical limitations:

- Lighting conditions can strongly affect results.
- Camera white balance and exposure can change measured colors.
- Background objects may produce false positives.
- A fixed threshold does not generalize reliably across all environments or skin tones.
- Color segmentation alone should not be used to infer identity, ethnicity, health status, or other personal characteristics.

## Future Improvements

Possible improvements include:

- Add adaptive thresholding for different lighting conditions.
- Compare multiple color spaces.
- Add morphological filtering and contour analysis.
- Add real-time FPS measurement.
- Create a simple graphical user interface.
- Add test images captured under varied lighting conditions.
- Compare rule-based segmentation with a trained segmentation model.
- Add quantitative evaluation using a labeled segmentation dataset.

## Responsible Use

This project should be used for educational computer vision experiments. Skin-color detection is sensitive to lighting, cameras, thresholds, and dataset coverage, so results should not be treated as reliable demographic or identity information.

## License

This repository includes the Boost Software License 1.0. See the `LICENSE` file for details.

## Author

Sithum Marasinghe
