# StructParts

**Seeing Both the Forest and the Trees: Reusing Holistic 3D Priors for Part-Decomposed Generation**

Yiqun Zhao¹˒², Binbin Huang¹˒², Haobin Duan¹˒², Zibo Zhao³, Shenghua Gao²˒⁴

¹ The University of Hong Kong · ² Transengram
³ Tencent Hunyuan · ⁴ Shenzhen Loop Area Institute

StructParts reuses a holistic 3D prior to generate detailed, structurally coherent part-decomposed objects from a segmented mesh scaffold.

This repository contains the static project homepage, pipeline and result figures, and a 15-second teaser film.

## Preview

```bash
python -m http.server 8000
```

## Publication

Keep this repository private during preparation. After the arXiv paper is live, update the paper links in `index.html`, make the GitHub repository public, and enable GitHub Pages from `main`, `/ (root)`. The intended URL is https://zhao-yiqun.github.io/structparts/.

## Model dependencies

DINOv2 checkpoints are not distributed with StructParts. Users download DINOv2-large directly from [facebook/dinov2-large](https://huggingface.co/facebook/dinov2-large). The inference release README documents setup. Our model artifacts contain only the diffusion transformer and VAE decoder.
