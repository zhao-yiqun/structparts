# StructParts

**Seeing Both the Forest and the Trees: Reusing Holistic 3D Priors for Part-Decomposed Generation**

**NeurIPS 2026**

Yiqun Zhao¹˒², Binbin Huang¹˒², Haobin Duan¹˒², Zibo Zhao³, Shenghua Gao¹˒²˒⁴*

¹ The University of Hong Kong · ² Transengram
³ Tencent · ⁴ Shenzhen Loop Area Institute

*Corresponding author: Shenghua Gao.*

StructParts reuses a holistic 3D prior to generate detailed, structurally coherent part-decomposed objects from a segmented mesh scaffold.

This repository contains the static project homepage, pipeline and result figures, and a 24-second teaser film.

## Preview

```bash
python -m http.server 8000
```

## Publication

The project homepage is https://zhao-yiqun.github.io/structparts/. GitHub Pages publishes from `main`, `/ (root)`. Update the paper link in `index.html` when the arXiv paper is available.

## Model dependencies

Our DiT and VAE decoder weights are hosted at [Goatzyq/structparts](https://huggingface.co/Goatzyq/structparts). See [the inference README](https://github.com/zhao-yiqun/structparts-code#setup) for download commands and setup. The model repository is private during preparation; private model downloads require an authorized Hugging Face login.

DINOv2 checkpoints are not distributed with StructParts. Users download DINOv2-large directly from [facebook/dinov2-large](https://huggingface.co/facebook/dinov2-large). The inference release README documents setup. Our model artifacts contain only the diffusion transformer and VAE decoder.

## Acknowledgments

We thank [Hunyuan3D-2.1](https://github.com/Tencent-Hunyuan/Hunyuan3D-2.1) and [UltraShape-1.0](https://github.com/PKU-YuanGroup/UltraShape-1.0) for their open-source models and implementations, which our work builds upon. Original license and copyright notices are retained in the inference code.

## Figure sources

The five static method/result figures are exported directly from the PDFs actively referenced by the paper, respecting each PDF’s saved CropBox. `figure-sources.json` records the LaTeX source, PDF SHA-256, crop coordinates, and output hashes. Re-export with `python scripts/site/export_paper_figures.py` in the paper repository, then sync the generated assets.
