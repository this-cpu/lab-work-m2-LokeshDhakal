## Title:  Fundamentals of digital image and basic image operations in Python

## Objectives:

1. Load and display digital images
2. Understand the digital image representation.
3. Color to grayscale and binary image translation.
4. Image transformation (Resize, Rotate, Flip).
5. Crop the ROI (Region of interest) in an image.

## Background Theory

- Digital Image representation    
- Color Models (RGB, Grayscale & Binary)
- Image File Formats
- Basic Image Transformation
- Introduction to OpenCV
    
## Procedure

### Read_n_display_img.ipynb
1. Loaded the original image using `cv2.imread()`.  
2. Displayed the image to verify it was correctly loaded.  
3. Checked basic properties such as height, width, channels, and data type.  

### Explore_image.ipynb
1. Explored the image properties in detail.  
2. Checked individual pixel values to understand intensity distribution.  
3. Confirmed the image dimensions and data type for further processing.  

### Image_Conversion.ipynb
1. Converted the original color image to **grayscale** to simplify the data to intensity values.  
2. Created a **binary image** using thresholding to highlight foreground and background.  
3. Saved both grayscale and binary images in BMP format to preserve data.  

### Image_Transformation.ipynb
1. Resized the original image to **300×300 pixels** to standardize dimensions for operations.  
2. Rotated the resized image by **45°** to demonstrate geometric transformation.  
3. Flipped the rotated image horizontally/vertically to demonstrate mirroring effects.  

### ROI_in_an_Image.ipynb
1. Displayed the original image to identify the desired region.  
2. Cropped a specific portion of the image to select the **Region of Interest (ROI)** for focused analysis.  

## Outputs

### Read_n_display_img.ipynb
- **Shape:** `(259, 194, 3)` → Indicates a color image with 3 channels (RGB)  
- **Data Type:** `uint8` → Each pixel value is stored as an 8-bit integer  
- **Pixel Value at (100,100):** `[75, 102, 146]` → Shows the red, green, and blue intensity of that pixel  
**Explanation:** Confirms that the image is correctly loaded and accessible for processing.  

### Explore_image.ipynb
- **Height:** 259  
- **Width:** 194  
- **Channels:** 3  
- **Data Type:** `uint8`  
**Explanation:** Verified image dimensions and color channels, ensuring compatibility with subsequent operations.  

### Image_Conversion.ipynb
- **Grayscale Image:** Single-channel image where each pixel represents intensity  
- **Binary Image:** Pixels are either 0 (black) or 255 (white) after thresholding  
**Explanation:** Grayscale simplifies intensity-based processing; binary image separates foreground from background for analysis.  

### Image_Transformation.ipynb
- **Resized Image:** 300×300 pixels, 3 channels, `uint8` → Maintains color while standardizing size  
- **Rotated Image:** Rotated by 45° → Demonstrates geometric manipulation  
- **Flipped Image:** Horizontally/vertically mirrored → Shows mirroring transformation  
**Explanation:** These transformations help in image normalization and augmentation for analysis or further processing.  

### ROI_in_an_Image.ipynb
- **Cropped Image:** Selected portion of the original image highlighting the ROI  
- **Explanation:** ROI allows focus on a specific part of the image, which is useful for detailed analysis or feature extraction.
  
## Conclusion

1. Successfully explored, converted, transformed, and cropped images.  
2. Demonstrated important image processing operations including:  
   - Grayscale and binary conversion  
   - Resizing, rotation, and flipping  
   - ROI selection  
3. Images were saved in **BMP format** to preserve quality for further analysis.
