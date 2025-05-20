# Neural Style Transfer with PyTorch  
A Python implementation of **Neural Style Transfer (NST)** using PyTorch and a pre-trained **VGG19** model. This technique blends the **content** of one image with the **artistic style** of another to create visually striking results.

## Project Details  
- **Company:** CODETECH IT SOLUTIONS  
- **Intern Name:** Aalay Kabariya
- **Intern ID:** C0DF49  
- **Domain:** Artificial Intelligence  
- **Duration:** 4 Weeks  
- **Mentor:** Neela Santosh  

## Features  
🖼 **Content-Style Fusion** – Combines a content image (e.g., a photo) with a style image (e.g., a painting).  
🎯 **Customizable Layers** – Uses specific **VGG19 layers** for style (conv1-4) and content (conv4).  
⚡ **Optimized Workflow** – Employs **L-BFGS optimizer** for efficient style transfer.  
🚀 **GPU Support** – Automatically leverages **CUDA** if available.  

## Technologies Used  
- **PyTorch** – Deep learning framework  
- **TorchVision** – Pre-trained VGG19 model & image transformations  
- **Pillow (PIL)** – Image loading & saving  
- **CUDA** – GPU acceleration (optional)  

## How It Works  
### Image Preprocessing  
✔ Resizes images to **256x256** and normalizes them for VGG19.  

### Model Setup  
✔ Loads pre-trained **VGG19 model** and extracts feature maps from specified layers.  

### Loss Calculation  
✔ **Content Loss** – Preserves the structure of the content image.  
✔ **Style Loss (Gram Matrix)** – Captures texture & color patterns from the style image.  

### Optimization  
✔ Iteratively updates the **generated image** using **L-BFGS optimizer** to minimize total loss.  

## Output  
### Sample Input  
🖼 _Content Image_  
🖼 _Style Image_ 
 ![Image](https://github.com/user-attachments/assets/d47d89b3-73b3-4161-8e08-3acf4c54f183)


### Generated Output  
![Image](https://github.com/user-attachments/assets/ca7298bb-e11b-473c-9a1c-23f3109d6df7)  

## Installation  
```bash
git clone https://github.com/yourusername/neural-style-transfer.git
cd neural-style-transfer
pip install torch torchvision pillow
