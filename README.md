# vakyansh-tts
Text to Speech for Indic languages

## 1. Installation and SetUp

Clone repo
```
git clone https://github.com/Open-Speech-EkStep/vakyansh-tts
```
Build conda virtual environment
```
cd ./vakyansh-tts
conda create --name <env_name> python=3.7
conda activate <env_name>
pip install -r requirements.txt
```
Install [apex](https://github.com/NVIDIA/apex); commit: 37cdaf4 for Mixed-precision training
```
cd ..
git clone https://github.com/NVIDIA/apex
cd apex
git checkout 37cdaf4
pip install -v --disable-pip-version-check --no-cache-dir ./
cd ../vakyansh-tts
```
Build Monotonic Alignment Search Code (Cython)
```
cd ./monotonic_align
python setup.py build_ext --inplace
cd ..
```
