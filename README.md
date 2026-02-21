<div align=center>
  <img src="./assets/logo.png" width=300 >
</div>

<h1>
  InfoDet: A Dataset for Infographic Element Detection
</h1>
<p align="center">
  <a href="https://openreview.net/forum?id=Wj0Sc9WBHZ">
    <img
      src="https://img.shields.io/badge/ICLR%202026-Paper-blue" 
      alt="InfoDet Paper on OpenReview"
    />
  </a>
  <a href="https://huggingface.co/datasets/InfoDet/InfoDet">
    <img
      src="https://img.shields.io/badge/InfoDet-Data-orange?logo=huggingface&logoColor=yellow" 
      alt="InfoDet data on Hugging Face"
    />
  </a>
</p>

> InfoDet is a dataset designed to support the development of accurate object detection models for charts and HROs in infographics. It contains 11,264 real and 90,000 synthetic infographics, with over 14 million bounding box annotations.

![TEASER](./assets/teaser.png)

## 🔥 News
- [2026.2] 🎉🎉 InfoDet has been accepted by **ICLR 2026**!
- [2025.11] 🎉🎉 We have released the first version of our dataset, which includes 11,264 real and 90,000 synthetic infographic charts, with over 14 million bounding box annotations.

## 📦 Dataset
**[👉 Access the full InfoDet dataset on Hugging Face 🤗! 👈](https://huggingface.co/datasets/InfoDet/InfoDet)**

InfoDet comprises a diverse collection of infographics from two sources: 1) real infographics collected from 7 online platforms, and 2) synthetic infographics programmatically created from 1,072 design templates.
To effectively annotate the infographics, we combine the model-in-the-loop and programmatic methods.

![PIPELINE](./assets/pipe.jpg)

## 🎯 Applications

The effectiveness of InfoDet is demonstrated through three applications:

### Thinking-with-Boxes via Grounded Chain-of-Thought

We construct a Thinking-with-Boxes scheme to enhance VLMs by explicitly providing grounded annotations of texts, charts, and HROs along with additional layered infographic images.
For more details, please refer to this [folder](grounded_CoT). 

![det_qual](./assets/GCoT.jpg)


### Evaluating Object Detection Models

We compare 11 object detection models on InfoDet to assess their performance in detecting charts and HROs. 
The following figure shows detection results of evaluated object detection models: (a) zero-shot prompting with DINO-X; (b) 4-shot prompting with T-Rex2; (c) 4-shot fine-tuning with Co-DETR; (d) fine-tuning on InfoDet with Co-DETR. Bounding boxes in colors are the predictions for charts and HROs.
For more details, please refer to this [folder](model_evaluation). 

![det_qual](./assets/det_qual.png)


### Applying the Developed Model to Graphic Layout Detection

To demonstrate the broader applicability of InfoDet, we evaluate its effectiveness on graphic layout detection tasks by applying the InternImage-based model.
For more details, please refer to this [folder](graphic_layout_detection). 


![det_qual](./assets/Graphic_det.png)


## ⚖️ License
This project is released under the [Apache 2.0 license](LICENSE).


## 📚 Citation

If you find our work helpful for your research, please consider citing the following BibTeX entry.

```bibtex
@inproceedings{
zhu2026infodet,
title={InfoDet: A Dataset for Infographic Element Detection},
author={Jiangning Zhu and Yuxing Zhou and Zheng Wang and Juntao Yao and Yima Gu and Yuhui Yuan and Shixia Liu},
booktitle={The Fourteenth International Conference on Learning Representations},
year={2026},
url={https://openreview.net/forum?id=Wj0Sc9WBHZ}
}
```


## ✨ Related Projects

- **ChartGalaxy: A Dataset for Infographic Chart Understanding and Generation**  
  [Paper](https://arxiv.org/abs/2503.00814) | [Code](https://github.com/Benny-Li-BI/ChartGalaxy) | [Dataset](https://huggingface.co/datasets/pengfeiliBI/ChartGalaxyDataset)
- **InfoChartQA: A Benchmark for Multimodal Question Answering on Infographic Charts**  
  [Paper](https://arxiv.org/abs/2503.08954) | [Code](https://github.com/YuxingZhou-thu/InfoChartQA) | [Dataset](https://huggingface.co/datasets/thu-vis/InfoChartQA)


## 🤝 Contact
- igraphicdet@outlook.com
