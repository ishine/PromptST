
# PromptST: Abstract Prompt Learning for End-to-End Speech Translation


This is an implementation of the EMNLP 2023 paper *"PromptST: Abstract Prompt Learning for End-to-End Speech Translation"* (read the paper [here](https://openreview.net/pdf?id=Nijnhwu1Uz)). 


## 👀 Overview
The motivation of our **PromptST** model is to broaden the abstract representation power of the encoder of S2T models.
<div align="left">
  <img src="https://github.com/ytf-philp/PromptST/assets/54100491/13025542-33c2-4f9b-b22e-3758c088f769" width="70%">
</div>


### Result on CoVoST En-X dataset
We report **case-sensitive detokenized BLEU** via the sacrebleu toolkit.

| Model      | En-De | En-Ca | En-Ar | En-Tr | Avg.  |
| ---------- |:-----:|:-----:|:-----:|:-----:|:-----:|
|Continue Train  |	25.9 |  33.3 |  19.3 | 17.6  |  24.0 |
|PromptST|  26.4 |  33.7 |  19.6 | 17.9  |  24.4 |

The BLEU score of adding PromptST to different layers on the dev set.
| Model      | En-De | En-Ca | En-Ar | En-Tr |
| ---------- |:-----:|:-----:|:-----:|:-----:|
|0-24 layers  |	29.9 |  36.7 |  23.5 | 20.4  |
|20-24 layers|  29.8 |  36.8 |  23.4 | 20.6  |
|16-24 layers|  29.9 |  36.5 |  23.7 | 20.5  |
|12-24 layers|  30.1 |  37.4 |  23.8 | 21.0  |
## Speech-Senteval Benchmark
  You can download the Speech-Senteval Benchmark at [Here](https://drive.google.com/file/d/1F-uXapnR1nJ1q81u1quBRtMv_-xJ564i/view?usp=share_link)

## ⬇️ Download Trained Models
The models are trained based on pytorch. 

|  |                                           **Model**                                            |   
|:--------:|:--------------------------------------------------------------------------------------:| 
| En-De    | [Download](https://huggingface.co/philip-xxf/PromptST-en-de) | 
| En-Ca    | [Download](https://huggingface.co/philip-xxf/PromptST-en-ca) | 
| En-Ar    | [Download](https://huggingface.co/philip-xxf/PromptST-en-ar) | 
| En-Tr    | [Download](https://huggingface.co/philip-xxf/PromptST-en-tr) | 



# All the code and scripts are still being updated and will be made public soon !!!

## Training & Generation Instruction
### ⚙️ Requirements and Installation
* [PyTorch](http://pytorch.org/) version >= 1.5.0
* Python version >= 3.6
* For training new models, you'll also need an NVIDIA GPU and [NCCL](https://github.com/NVIDIA/nccl)
```bash
git clone git@github.com:ytf-philip/PromptST.git
cd PromptST
pip3 install -r requirements.txt
```

### Probing Task Analysis
```bash

```

### Training, Inference, Generation and Evaluation
To train the model, take En-De as an example; you may run:
```bash

```
```bash

```


## Citation
```

```
## License
[License](#license)
