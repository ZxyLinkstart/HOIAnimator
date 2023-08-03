# HOIAnimator: Text-Driven Human-Object Animations with Interactive Diffusion Models

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
conda activate mdm
python -m spacy download en_core_web_sm
pip install git+https://github.com/openai/CLIP.git
```

Download dependencies:

<details>
  <summary><b>Text to Motion</b></summary>

```bash
bash prepare/download_smpl_files.sh
bash prepare/download_glove.sh
bash prepare/download_t2m_evaluators.sh
```
</details>

<details>
  <summary><b>Action to Motion</b></summary>

```bash
bash prepare/download_smpl_files.sh
bash prepare/download_recognition_models.sh
```
</details>

<details>
  <summary><b>Unconstrained</b></summary>

```bash
bash prepare/download_smpl_files.sh
bash prepare/download_recognition_models.sh
bash prepare/download_recognition_unconstrained_models.sh
```
</details>



python -m train.train_mdm --save_dir ./save/body_obj_final  --vertice 1  --dataset humanml 


python -m train.train_mdm --save_dir ./save/ori_0802  --dataset humanml

python -m train.train_mdm --save_dir ./save/vertice_final_1_1  --vertice 1 --dataset humanml 

00:
'a person holds a backpack'
01:
'a person types on a keyboard'
02:
'a person touches a wood chair'
03:
'a person sits on a wood chair'
04:
'a person lifts a long box'
05:
'a person holds a large box'
06:
'a person lifts a plastic container'
07:
'a person touches a suitcase'
08:
'a person lifts a black chair'
09:
'a person touches a black chair'
10:
'a person lifts a wood chair'
11:
'a person sits on a yogaball'
12:
'a person lifts a toolbox'
13:
'a person moves a monitor'
14:
'a person moves a stool'
15:
'a person lifts a small box'
16:
'a person holds a medium box'
17:
'a person touches a square table'
18:
'a person leans on a small table'
19:
'a person lifts a small table'
20:
'a person touches a yogamat'
21:
'a person touches a monitor'
22:
'a person sits on a square table'
23:
'a person lifts a trashbin'
24:
'a person sits on a stool'
25:
'a person carries a backpack'
26:
'a person moves a small table'
27:
'a person lifts a tiny box'
28:
'a person touches a backpack'
29:
'a person moves a keyboard'
30:
'a person lifts a suitcase'
31:
'a person plays with a yogaball'