## Focus-DETR
This is the official implementation of the paper "Less is More: Focus Attention for Efficient DETR" 

Authors: Dehua Zheng, Wenhui Dong, Hailin Hu, Xinghao Chen, Yunhe Wang.

[[`arXiv`](https://arxiv.org/abs/2307.12612)] [[`BibTeX`](#citing-focus-detr)]

Focus-DETR is a model that focuses attention on more informative tokens for a better trade-off between computation efficiency and model accuracy. Compared with the state-of-the-art sparse transformed-based detector under the same setting, our Focus-DETR gets comparable complexity while achieving 50.4AP (+2.2) on COCO.

<div align="center">
  <img src="./assets/overview.jpg"/>
</div><br/>

## Table of Contents
- [Focus-DETR](#focus-detr)
- [Table of Contents](#table-of-contents)
- [Main Results with Pretrained Models](#main-results-with-pretrained-models)
    - [Pretrained focus\_detr with ResNet Backbone](#pretrained-focus_detr-with-resnet-backbone)
    - [Pretrained focus\_detr with Swin-Transformer Backbone](#pretrained-focus_detr-with-swin-transformer-backbone)
- [Installation](#installation)
- [Training](#training)
- [Evaluation](#evaluation)

## Main Results with Pretrained Models

Here we provide the pretrained `Focus-DETR` weights based on detrex.

##### Pretrained focus_detr with ResNet Backbone

<table><tbody>
<!-- START TABLE -->
<!-- TABLE HEADER -->
<th valign="bottom">Name</th>
<th valign="bottom">Backbone</th>
<th valign="bottom">Pretrain</th>
<th valign="bottom">Epochs</th>
<th valign="bottom">Denoising Queries</th>
<th valign="bottom">box<br/>AP</th>
<th valign="bottom">download</th>
<!-- TABLE BODY -->
<!-- ROW: focus_detr_r50_4scale_12ep -->
 <tr><td align="left"><a href="configs/focus_detr_resnet/focus_detr_r50_4scale_12ep.py">Focus-DETR-R50-4scale</a></td>
<td align="center">R-50</td>
<td align="center">IN1k</td>
<td align="center">12</td>
<td align="center">100</td>
<td align="center">48.8</td>
<td align="center"> <a href="https://github.com/linxid/Focus-DETR-mindspore/releases/download/Focus-DETR/focus_detr_r50_4scale_12ep.zip">model</a></td>
</tr>
<!-- ROW: focus_detr_r50_4scale_24ep -->
 <tr><td align="left"><a href="configs/focus_detr_resnet/focus_detr_r50_4scale_24ep.py">Focus-DETR-R50-4scale</a></td>
<td align="center">R-50</td>
<td align="center">IN1k</td>
<td align="center">24</td>
<td align="center">100</td>
<td align="center">50.3</td>
<td align="center"> <a href="https://github.com/linxid/Focus-DETR-mindspore/releases/download/Focus-DETR/focus_detr_r50_4scale_24ep.zip">model</a></td>
</tr>
<!-- ROW: focus_detr_r50_4scale_36ep -->
 <tr><td align="left"><a href="configs/focus_detr_resnet/focus_detr_r50_4scale_36ep.py">Focus-DETR-R50-4scale</a></td>
<td align="center">R-50</td>
<td align="center">IN1k</td>
<td align="center">36</td>
<td align="center">100</td>
<td align="center">50.4</td>
<td align="center"> <a href="https://github.com/linxid/Focus-DETR-mindspore/releases/download/Focus-DETR/focus_detr_r50_4scale_36ep_v3.zip">model</a></td>
</tr>
<!-- ROW: focus_detr_r101_4scale_12ep -->
 <tr><td align="left"><a href="configs/focus_detr_resnet/focus_detr_r101_4scale_12ep.py">Focus-DETR-R101-4scale</a></td>
<td align="center">R-101</td>
<td align="center">IN1k</td>
<td align="center">12</td>
<td align="center">100</td>
<td align="center">50.8</td>
<td align="center"> <a href="https://github.com/linxid/Focus-DETR-mindspore/releases/download/Focus-DETR/focus_detr_r101_4scale_12ep.zip">model</a></td>
</tr>
<!-- ROW: focus_detr_r101_4scale_24ep -->
 <tr><td align="left"><a href="configs/focus_detr_resnet/focus_detr_r101_4scale_24ep.py">Focus-DETR-R101-4scale</a></td>
<td align="center">R-101</td>
<td align="center">IN1k</td>
<td align="center">24</td>
<td align="center">100</td>
<td align="center">51.2</td>
<td align="center"> <a href="https://github.com/linxid/Focus-DETR-mindspore/releases/download/Focus-DETR/focus_detr_r101_4scale_24ep.zip">model</a></td>
</tr>
<!-- ROW: focus_detr_r101_4scale_36ep -->
 <tr><td align="left"><a href="configs/focus_detr_resnet/focus_detr_r101_4scale_36ep.py">Focus-DETR-R101-4scale</a></td>
<td align="center">R-101</td>
<td align="center">IN1k</td>
<td align="center">36</td>
<td align="center">100</td>
<td align="center">51.4</td>
<td align="center"> <a href="https://github.com/linxid/Focus-DETR-mindspore/releases/download/Focus-DETR/focus_detr_r101_4scale_36ep_v2.zip">model</a></td>
</tr>
</tbody></table>

#### Pretrained focus_detr with Swin-Transformer Backbone

<table><tbody>
<th valign="bottom">Name</th>
<th valign="bottom">Backbone</th>
<th valign="bottom">Pretrain</th>
<th valign="bottom">Epochs</th>
<th valign="bottom">Denoising Queries</th>
<th valign="bottom">box<br/>AP</th>
<th valign="bottom">download</th>
<!-- ROW: focus_detr_swin_tiny_4scale_12ep -->
<tr><td align="left"><a href="configs/focus_detr_swin/focus_detr_swin_tiny_224_4scale_12ep.py">Focus-DETR-Swin-T-224-4scale</a></td>
<td align="center">Swin-Tiny-224</td>
<td align="center">IN1k</td>
<td align="center">12</td>
<td align="center">100</td>
<td align="center">50.0</td>
<td align="center"> <a href="https://github.com/linxid/Focus-DETR-mindspore/releases/download/Focus-DETR/focus_detr_swin_tiny_224_4scale_12ep.zip">model</a></td>
</tr>
<!-- ROW: focus_detr_swin_tiny_4scale_24ep -->
<tr><td align="left"><a href="configs/focus_detr_swin/focus_detr_swin_tiny_224_4scale_24ep.py">Focus-DETR-Swin-T-224-4scale</a></td>
<td align="center">Swin-Tiny-224</td>
<td align="center">IN1k</td>
<td align="center">24</td>
<td align="center">100</td>
<td align="center">51.2</td>
<td align="center"> <a href="https://github.com/linxid/Focus-DETR-mindspore/releases/download/Focus-DETR/focus_detr_swin_tiny_224_4scale_24ep.zip">model</a></td>
</tr>
<!-- ROW: focus_detr_swin_tiny_4scale_36ep -->
<tr><td align="left"><a href="configs/focus_detr_swin/focus_detr_swin_tiny_224_4scale_36ep.py">Focus-DETR-Swin-T-224-4scale</a></td>
<td align="center">Swin-Tiny-224</td>
<td align="center">IN1k</td>
<td align="center">36</td>
<td align="center">100</td>
<td align="center">52.5</td>
<td align="center"> <a href="https://github.com/IDEA-Research/detrex-storage/releases/download/v0.1.1/focus_detr_swin_tiny_224_4scale_12ep.pth">model</a></td>
</tr>
<!-- ROW: focus_detr_swin_tiny_4scale_22k_36ep -->
<tr><td align="left"><a href="configs/focus_detr_swin/focus_detr_swin_tiny_224_4scale_36ep.py">Focus-DETR-Swin-T-224-4scale</a></td>
<td align="center">Swin-Tiny-224</td>
<td align="center">IN22k to IN1k</td>
<td align="center">36</td>
<td align="center">100</td>
<td align="center">53.2</td>
<td align="center"> <a href="">model</a></td>
</tr>
<!-- ROW: focus_detr_swin_base_4scale_22k_36ep -->
<tr><td align="left"><a href="configs/focus_detr_swin/focus_detr_swin_base_384_4scale_36ep.py">Focus-DETR-Swin-B-384-4scale</a></td>
<td align="center">Swin-Base-384</td>
<td align="center">IN22k to IN1k</td>
<td align="center">36</td>
<td align="center">100</td>
<td align="center">56.2</td>
<td align="center"> <a href="https://github.com/linxid/Focus-DETR-mindspore/releases/download/Focus-DETR/focus_detr_swin_base_384_4scale_22k_36ep.pth">model</a></td>
</tr>
<!-- ROW: focus_detr_swin_large_4scale_22k_36ep -->
<tr><td align="left"><a href="configs/focus_detr_swin/focus_detr_swin_large_384_4scale_36ep.py">Focus-DETR-Swin-L-384-4scale</a></td>
<td align="center">Swin-Large-384</td>
<td align="center">IN22k to IN1k</td>
<td align="center">36</td>
<td align="center">100</td>
<td align="center">56.3</td>
<td align="center"> <a href="">model</a></td>
</tr>
</tbody></table>

**Note:**
* Swin-X-384 means the backbone pretrained resolution is 384 x 384 and IN22k to In1k means the model is pretrained on ImageNet-22k and finetuned on ImageNet-1k.

## Installation
Please refer to [Installation Instructions](https://detrex.readthedocs.io/en/latest/tutorials/Installation.html) for the details of installation.

## Training
All configs can be trained with:

```bash
cd detrex
python tools/train_net.py --config-file projects/focus_detr/configs/path/to/config.py --num-gpus 8
```
By default, we use 8 GPUs with total batch size as 16 for training.

## Evaluation
Model evaluation can be done as follows:
```bash
cd detrex
python tools/train_net.py --config-file projects/focus_detr/configs/path/to/config.py --eval-only train.init_checkpoint=/path/to/model_checkpoint
```

## Citing Focus-DETR
If you find our work helpful for your research, please consider citing the following BibTeX entry.

```BibTex
@misc{zheng2023more,
      title={Less is More: Focus Attention for Efficient DETR}, 
      author={Dehua Zheng and Wenhui Dong and Hailin Hu and Xinghao Chen and Yunhe Wang},
      year={2023},
      eprint={2307.12612},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
【This open source project is not an official Huawei product, Huawei is not expected to provide support for this project.】