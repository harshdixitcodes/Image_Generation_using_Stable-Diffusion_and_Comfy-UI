# IMAGE GENERATION USING COMFY UI AND STABLE DIFFUSION

This project is part of the AICTE Internship on AI: Transformative Learning with TechSaksham – A joint CSR initiative of Microsoft & SAP. It demonstrates the utilization of Stable Diffusion and ComfyUI for generating images from text prompts. ComfyUI’s node-based interface enables flexible and intuitive image generation workflows, making Stable Diffusion more accessible and customizable.

---

## Table of Contents
- Introduction
- Features
- Requirements
- Installation
- Usage

---

## Introduction
Stable Diffusion is an advanced deep learning model designed to generate high-quality images based on textual descriptions. ComfyUI enhances usability by offering a visual programming environment where users can create and modify image generation pipelines with ease. This project integrates these tools to provide an efficient and interactive image generation experience.

---

## Features
- **Visual Workflow Design:** Utilize ComfyUI’s intuitive node-based system to build and customize image generation pipelines.
- **Text-to-Image Generation:** Generate images based on text descriptions using Stable Diffusion.
- **Customizable Parameters:** Modify various parameters within ComfyUI to control the style and details of the generated images.
- **Modular Design:** Easily add, remove, or reorganize nodes in ComfyUI to experiment with different image processing techniques.
- **Real-time Feedback:** (If supported by ComfyUI) Preview images while adjusting parameters for a faster creative process.
- **Extensibility:** Integrate additional Python scripts and custom nodes into ComfyUI for enhanced functionality.

---

## Requirements

### Hardware
- **Operating System:** Windows 10/11, macOS, or Linux (Linux recommended for best performance).
- **Processor (CPU):** Multi-core CPU for smooth performance.
- **Graphics Card (GPU):** NVIDIA GPU with at least 8GB VRAM (12GB+ recommended); AMD GPUs require additional configuration.
- **Memory (RAM):** Minimum 16GB RAM (32GB+ recommended for optimal performance).
- **Storage:** SSD with sufficient storage capacity.

### Software
- **Python:** Version 3.8+ (recommended: 3.10 or 3.11).
- **ComfyUI:** Download and install from the official GitHub repository.
- **Stable Diffusion Model Checkpoint:** Download a compatible model file (.ckpt or .safetensors).
- **Required Python Libraries:**
  - `torch`, `torchvision`, `torchaudio` (for PyTorch)
  - `transformers`, `numpy`, `Pillow`, `Flask`, `requests`, `tqdm`, `filelock`, `gradio`, `omegaconf`

---

## Installation

### Step 1: Install Python
Ensure Python 3.8 or higher is installed. Versions 3.10 or 3.11 are preferred for stability.

### Step 2: Install ComfyUI
Clone the official ComfyUI repository to a local directory. Follow the setup instructions provided in the repository to complete the installation.

### Step 3: Download Stable Diffusion Model
Download the `v1-5-pruned-emaonly-fp16` model from Hugging Face. (Provide a link if applicable.)

### Step 4: Place Model Checkpoint
Move the downloaded model file to the following directory inside the ComfyUI installation:
```
ComfyUI_windows_portable\ComfyUI\models\checkpoints
```
Ensuring the correct placement of the model file is essential for ComfyUI to detect and load it.

### Step 5: Install Dependencies
Navigate to the ComfyUI directory in a terminal or command prompt and set up a virtual environment (recommended for dependency management):
```
python3 -m venv .venv  # Create a virtual environment
source .venv/bin/activate  # Activate (Linux/macOS)
.venv\Scripts\activate  # Activate (Windows)
```
Then, install the required Python libraries:
```
pip install torch torchvision torchaudio transformers numpy Pillow Flask requests tqdm filelock gradio omegaconf
```
(Ensure the PyTorch installation matches your CUDA version for best performance on an NVIDIA GPU.)

### Step 6: Run ComfyUI
Launch ComfyUI as per the documentation. Since the model checkpoint is placed in the correct directory, ComfyUI will automatically recognize and load it.

---

## Usage
1. **Run ComfyUI**: Start the application as per the official documentation.
2. **Load Workflow (Optional)**: If a pre-designed workflow exists, load it. Otherwise, create a new workflow from scratch.
3. **Input Prompt**: Enter a text description in the appropriate node within ComfyUI.
4. **Adjust Parameters**: Modify node settings to refine the image generation process.
5. **Generate Image**: Execute the workflow to generate the desired image.
6. **View Results**: The generated image will be displayed within ComfyUI.

By following these steps, you can effectively create and modify images using Stable Diffusion and ComfyUI, leveraging the power of AI-driven text-to-image generation.
