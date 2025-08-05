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


Finally, this work has been extended for journal submission, with new modules introduced to generate more refined HOI animations. The complete implementation will be fully open‑sourced upon submission.

（Since I have graduated with a master's degree and my research direction has changed, my junior has taken over the job. I'm sorry to have kept you waiting for so long.）
