**Github link**

https://github.com/lihanwen1017769643/QANet

**demo link**

https://www.youtube.com/watch?v=MpwO--u1eW8

**create conda env**

`conda env create -f environment.yml`

`pip install torch==1.10.0+cu102 torchvision==0.11.0+cu102 torchaudio==0.10.0 -f https://download.pytorch.org/whl/torch_stable.html`

`pip install absl-py`

`pip install spacy==3.6.1`

**download data**

`sh download.sh`

**preprocess data**

`python3 config.py --mode prepro`

**train (with cuda)**

`python3 QANet_main.py --batch_size 4 --epochs 30 --with_cuda --use_ema`

Note: Aruguments in the training procedure can be altered. Details are defined in `QANet_main.py.`
