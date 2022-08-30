# T5-transformer
<p align="center">
  <img src="https://github.com/CosimoGiani/T5-transformer/blob/main/images/t5%20framework.gif" style="width:600px;">
</p>
<p align="center">
    <em>Source: Google AI Blog<sup class="footnote-ref"><a href="#fn1" id="fnref1">[1]</a></sup></em>
</p>


## About The Project
Study of the methodology proposed in the paper [Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer](https://arxiv.org/abs/1910.10683).

In this project one of the T5 models - precisely **T5-small** - is fine-tuned over a fraction of the tasks performed in the paper. In addition, to further extend this work it was tested the **adapter layers** variant for fine-tuning. 

More details about the project in the [presentation](presentation.pdf).

### Built With
* [:hugs: Transformers](https://github.com/huggingface/transformers)
* [PyTorch](https://pytorch.org/)
* <img align="center" height="30" src="https://raw.githubusercontent.com/Adapter-Hub/adapter-transformers/master/adapter_docs/logo.png"> [Adapter Transformers](https://github.com/adapter-hub/adapter-transformers)

## Usage
In the repo there are two notebooks, one for "standard" fine-tuning and one for fine-tuning with adapters. To facilitate reading, the notebooks follow the pipeline for the question-answering task. Despite this, the implementations are totally generalizable to all types of tasks.
1. Execute ```t5-fine-tune.ipynb``` to fine-tune the model. In order to change task, it might be necessary to make small adjustments in the *pre-processing* setup.
2. Execute ```t5-fine-tune-adapters.ipynb``` to fine-tune the model with the adapters. To manipulate the inner dimensionality of the adapter layer it is sufficient to change properly the value of the *reduction factor*.

## Acknowledgments
<ol class="footnotes-list">
<li id="fn1" class="footnote-item"><p>The image has been taken from this <a href="https://ai.googleblog.com/2020/02/exploring-transfer-learning-with-t5.html">Google AI Blog</a>.</p>
</li>
</ol>
