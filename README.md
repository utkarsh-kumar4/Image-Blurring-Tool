# 🖼️ Image Blurring Tool

## 👋 Hi there! Utkarsh here :p
Welcome to the Image Blurring Tool! This project helps you easily blur images using a simple mean filter. Enjoy smoothening your images with just a few clicks!

## 🌟 Features
- **Blurring**: Smoothens images by averaging pixel values within a specified neighborhood.
- **Compatibility**: Handles both grayscale and RGB images seamlessly.

## 🚀 Usage

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/utkarsh-kumar4/Image-Blurring-Tool.git
   cd image-blur-tool
   ```

2. **Run the Blur Function:**
   ```matlab
   output = blur('image_path[with extension]', blur_width);
   ```

   - `image_path[with extension]`: Path to the image file.
   - `blur_width`: Width of the blur filter (e.g., `1` for a 3x3 filter).

## 📷 Example

```matlab
blurred_image = blur('example_image.jpg', 2);
imshow(blurred_image);
```

## 👨🏻‍💻 Code Explanation

This MATLAB tool performs image blurring using a mean filter. The core function `blur(img, w)` takes an image file and a blur width `w` as input. 

1. **Loading the Image**: The image is read using `imread`. If the image is in color (RGB), it processes each channel (Red, Green, Blue) separately; otherwise, it processes the grayscale image directly.

2. **Creating Output Image**: For each pixel in the image, a sub-matrix of size `(2w+1) x (2w+1)` centered on the pixel is extracted. 

3. **Calculating Mean**: The mean of the pixel values within this sub-matrix is computed and assigned to the corresponding pixel in the output image.

4. **Handling Edge Cases**: For pixels near the edges, the sub-matrix is adjusted to avoid going out of bounds.

5. **Displaying the Result**: The processed image is converted to an 8-bit unsigned integer format and displayed using `imshow`.

The blurring effect smooths the image by averaging pixel values, reducing high-frequency noise and details.

## 🖼️ Image Comparison
<table>
  <tr>
    <td>
      <strong>Original Image of the 🐐👑</strong><br>
      <img src="https://github.com/utkarsh-kumar4/Image-Blurring-Tool/blob/main/messi.png" width="400" alt="Original Image">
    </td>
    <td>
      <strong>Blurred Image of the 🐐👑 [w = 10]</strong><br>
      <img src="https://github.com/utkarsh-kumar4/Image-Blurring-Tool/blob/main/messi_blurred.png" width="400" alt="Blurred Image">
    </td>
  </tr>
</table>

## 🛠️ Dependencies
- MATLAB (R2018b or later)

## 👤 Author
[Utkarsh Kumar](https://github.com/utkarsh-kumar4) 👨🏻‍💻🎓
