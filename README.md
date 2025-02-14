
# Image Generation Using Stable Diffusion & ComfyUI

This repository explores Stable Diffusion, a powerful AI model for generating high-quality images, and ComfyUI, a modular node-based interface that enhances control and customization.




## System Requirements

Before installing, ensure your system meets the following:

✅ GPU: NVIDIA (RTX 2060 or higher recommended) with CUDA support

✅ VRAM: 4GB+ (8GB+ recommended)

✅ OS: Windows 10/11 or Linux (Ubuntu, Arch, etc.)

✅ Python: Version 3.10+

✅ CUDA & cuDNN: Installed for GPU acceleration

✅ Python and Git extensions


## Installation

Clone ComfyUI Repository
```bash
git clone https://github.com/comfyanonymous/ComfyUI.git
cd ComfyUI

```
Create and Activate Virtual Environment

```bash
# Create virtual environment
python -m venv venv

# On Windows
venv\Scripts\activate

# On Linux/Mac
source venv/bin/activate

```
Install Dependencies
```bash
pip install -r requirements.txt

#If you encounter issues with missing libraries (like torch, numpy, etc.), you can install them manually

```
Download Stable Diffusion Model
```bash
https://huggingface.co/Comfy-Org/stable-diffusion-v1-5-archive/blob/main/v1-5-pruned-emaonly-fp16.safetensors

#You can download other models from:
#Hugging Face
#CivitAI
```
Place the Stable Diffusion model file (.safetensors or .ckpt)
```bash
ComfyUI/
├── models/
│   └── checkpoints/
│       └── model.ckpt  (the downloaded Stable Diffusion .ckpt file or .safetensors file)
```

```bash

```
    
## Run ComfyUI

Once everything is set up, run the following command inside the ComfyUI folder:

```bash
python main.py

```


This will start ComfyUI, and you can access it in your browser at: 

```bash
http://127.0.0.1:5000

```

```bash
Enter a text prompt into the input field.
Press "Generate" to produce the image based on your prompt.

```




## WorkFlow

![Workflow](https://github.com/Khushijain83037/Image-Generation-using-stable-diffusion-Comfy-UI-/blob/main/images/WorkFlow.png?raw=true)


## Running Tests

Run the Prompt

```bash
 A majestic lion roaring in the wild, with golden fur and piercing eyes, standing on a cliff during sunset

```


## Output

![Output](https://github.com/Khushijain83037/Image-Generation-using-stable-diffusion-Comfy-UI-/blob/main/images/ComfyUI_00030_.png?raw=true)


## Test 2

Run the Prompt

```bash
 A surreal underwater scene with colorful fish swimming around coral reefs, with light filtering from above the water.

```


## Output 2

![Output](https://github.com/Khushijain83037/Image-Generation-using-stable-diffusion-Comfy-UI-/blob/main/images/ComfyUI_00031_.png?raw=true)


## Troubleshooting
"RuntimeError: Numpy is not available"
This error can occur if numpy is not installed. You can fix this by installing it via:

```
pip install numpy==1.26.4
```

"ModuleNotFoundError: No module named 'safetensors'"
This indicates that the safetensors package is missing. Install it using:


```
pip install safetensors

```

```
"Model not found" error
Ensure the checkpoint model is correctly placed in the models directory and is named correctly. Update your configuration if necessary.

```
## Optimizations

1️⃣ Use Low VRAM Optimization

2️⃣ Optimize Batch Processing

3️⃣ Reduce Model Size with VAEs

4️⃣ Enable CUDA Graphs for Speedup

5️⃣ Use Efficient Samplers

6️⃣ Optimize for CPU Users


## Demo Video

[🎥 Watch the demo](https://github.com/Khushijain83037/Image-Generation-using-stable-diffusion-Comfy-UI-/blob/main/Demo/Demo.mp4)


## Credits

 - [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
 - [Stable Diffusion Models](https://huggingface.co/Comfy-Org/stable-diffusion-v1-5-archive/blob/main/v1-5-pruned-emaonly-fp16.safetensors)
 - [Python](https://www.python.org/)

### About Me  
I'm **Khushi Jain**, a **BTech 3rd-year student** with experience in **Frontend & Backend Development**.  
I am familiar with:  
- **Frontend**: HTML, CSS, ReactJS  
- **Backend**: PHP, Java  
- **Database**: SQL  
## 🔗 Links

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/khushi-jain-570a3a271/)

