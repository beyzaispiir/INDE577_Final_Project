# 📦 Image Compression with Singular Value Decomposition (SVD)

In this project, I applied **Singular Value Decomposition (SVD)** for compressing an image while preserving its visual quality.  
SVD is a powerful matrix factorization technique that can efficiently reduce the size of an image by approximating it with fewer singular values.  
Additionally, I visualized the separate Red, Green, and Blue (RGB) channels of the image to better understand how the compression process works at the pixel level.

As a personal touch, I used a photo of my own cat, **Peynir**, who just turned one year old. I miss her very much! 🐱❤️

---

## 🛠️ Algorithms Implemented

- **Singular Value Decomposition (SVD):**  
  Decomposing the Red, Green, and Blue channels of the image separately using SVD.
  
- **Image Compression:**  
  Reconstructing the image with a reduced number of singular values (`k`) to achieve compression.
  
- **Compression Ratio Calculation:**  
  Quantifying the reduction in data storage compared to the original image.

- **Bonus Visualization:**  
  Displaying each individual color channel (Red, Green, Blue) separately.

- **Interactive Compression (Optional):**  
  Using an interactive slider to dynamically adjust the compression rank if `ipywidgets` is installed.

---

## 🖼️ Dataset Used

- **Image:**  
  A real-world RGB image named `peynir.jpg`, showing my cat.

- **Image Details:**
  - Size: 2048 × 1536 pixels
  - Channels: 3 (Red, Green, Blue)

*You can replace it with your own image by placing your `.jpg` file in the same directory and updating the file name in the code.*

---

## 🧩 Instructions to Reproduce the Results

1. **Install Necessary Libraries**

   Make sure you have the following Python libraries installed:

   ```bash
   pip install numpy matplotlib ipywidgets
2. **Place Your Image**

Put your image file (e.g., your_image.jpg) in the same directory as the notebook.

3. **Update the File Name**

In the code cell where the image is loaded, replace:
img = imread('your_image.jpg')

4. **Run the Notebook Step-by-Step**

The notebook performs the following actions:

- 📥 **Load and display the original image**
- 🌈 **Separate the RGB channels** (Red, Green, Blue)
- 📐 **Apply Singular Value Decomposition (SVD)** to each color channel
- 🛠 **Reconstruct compressed versions** for various values of `k` (number of singular values)
- 🖼 **Visualize the compression effects** to assess quality vs. compression trade-off
- 🌈 **(Bonus)**: Visualize each RGB channel separately
- 🎛 **(Bonus)**: Use interactive sliders to explore compression dynamically (requires `ipywidgets`)

---

## 🎯 Key Learning Points

- **SVD is a powerful tool** for image compression, allowing significant size reduction with minimal visual loss.
- **Tuning `k`** helps control the balance between **compression rate** and **image quality**.
- **RGB channel separation** provides deeper insight into how each color contributes to the final image.
- **Scaling pixel values** to the range [0, 1] ensures better numerical performance during matrix operations.
- **Interactive compression** via sliders makes exploration of compression effects much more intuitive and engaging.
