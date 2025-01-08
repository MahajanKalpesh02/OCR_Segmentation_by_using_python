# Readmefile for OCR with Word-Level And Line-Level Segmentation

This project demonstrates how to perform Optical Character Recognition (OCR) on an image using Tesseract and OpenCV in Python. The script processes an image to extract text and visualize word-level bounding boxes.

---

## Requirements

Before running the script, ensure you have the required libraries and tools installed. Below is a list of the dependencies with a brief description and installation commands.

### Python Libraries

1. **OpenCV**:
   - OpenCV is used for image processing, such as converting images to grayscale and applying thresholding.
   - Installation Command:
     ```bash
     pip install opencv-python
     ```

2. **pytesseract**:
   - pytesseract is a Python wrapper for Google Tesseract-OCR Engine. It performs the text extraction from images.
   - Installation Command:
     ```bash
     pip install pytesseract
     ```

3. **matplotlib**:
   - matplotlib is used for plotting and visualizing the image with bounding boxes.
   - Installation Command:
     ```bash
     pip install matplotlib
     ```

### External Tool

4. **Tesseract-OCR**:
   - Tesseract is an open-source OCR engine required for text recognition. Ensure it is installed and added to your system’s PATH.
   - Installation Commands:
     - On Ubuntu:
       ```bash
       sudo apt update
       sudo apt install tesseract-ocr
       ```
     - On macOS (using Homebrew):
       ```bash
       brew install tesseract
       ```
     - On Windows:
       - Download and install Tesseract from [here](https://github.com/tesseract-ocr/tesseract).
       - Add the installation path to the system’s PATH environment variable.

---

## Usage Instructions

1. Place your image file in the project directory and update the `image_path` variable in the script with your image's filename.

2. Run the script using:
   ```bash
   python script_name.py
   ```
   Replace `script_name.py` with the actual name of your Python file.

3. The script will:
   - Convert the image to grayscale.
   - Apply thresholding for better OCR results.
   - Perform OCR to detect text and extract word-level bounding boxes.
   - Display the image with bounding boxes around each detected word.

---

## Output

- A visualization of the input image with word-level bounding boxes drawn around the detected text.
- Each word is annotated with its extracted text and bounding box.

---

## Notes

- Ensure the Tesseract executable is accessible from your system’s PATH.
- Use high-quality images for better OCR accuracy.
- Modify the `custom_config` variable to experiment with different Tesseract page segmentation modes (PSM).

