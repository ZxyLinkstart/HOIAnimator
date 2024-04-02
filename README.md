# HOIAnimator: Text-Driven Human-Object Animations with Interactive Diffusion Models [CVPR24]

## Getting started

This code was tested on `Ubuntu 18.04.5 LTS` and requires:

* Python 3.7
* conda3 or miniconda3
* CUDA capable GPU (one is enough)

### 1. Setup environment

Install ffmpeg (if not already installed):

```shell
sudo apt update
sudo apt install ffmpeg
```

Setup conda env:
```shell
conda env create -f environment.yml
conda activate HOIAnimator
python -m spacy download en_core_web_sm
pip install git+https://github.com/openai/CLIP.git
```
Coming soon!!!!
