## 🖼️ Image Blurring Tool

This MATLAB tool performs image blurring using a mean filter. It effectively processes both color (RGB) and grayscale images.

### 🌟 Features
- **Blurring**: Smoothens images by averaging pixel values within a specified neighborhood.
- **Compatibility**: Handles both grayscale and RGB images seamlessly.

### 🚀 Usage

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/image-blur-tool.git
   cd image-blur-tool
   ```

2. **Run the Blur Function:**
   ```matlab
   output = blur('path_to_image.jpg', blur_width);
   ```

   - `path_to_image.jpg`: Path to the image file.
   - `blur_width`: Width of the blur filter (e.g., `1` for a 3x3 filter).

### 📷 Example

```matlab
blurred_image = blur('example_image.jpg', 2);
imshow(blurred_image);
```

### 🔍 How It Works

1. **Load Image**: Reads the image file and processes each color channel separately if it's an RGB image.
2. **Create Output**: Extracts a sub-matrix around each pixel based on the blur width.
3. **Calculate Mean**: Computes the average of pixel values within the sub-matrix for blurring.
4. **Handle Edges**: Adjusts sub-matrices for edge pixels to prevent out-of-bounds errors.
5. **Display**: Converts the output to 8-bit format and displays it.

### 🛠️ Dependencies
- MATLAB (R2018b or later)

### 📜 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

### 👤 Author
[Your Name](https://github.com/yourusername)

---

Feel free to adjust the content to better fit your project or personal style!
