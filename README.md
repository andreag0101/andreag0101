### Hi, I'm Andrea Goh

AI/ML engineer and computer vision researcher. I like taking a system apart down to the math, rebuilding it from scratch, and shipping the result — not just calling a library and moving on.

- 🔭 Currently an **AI Development Intern at ArgonDigital**, building RAG-based LLM applications on AWS Bedrock
- 🔬 Computer Vision Research Assistant at **Purdue's Robotic Vision Lab** — multimodal transformers and 3D reconstruction pipelines built from classical vision theory, no OpenCV
- 🎓 M.S. Computer Engineering (AI/ML) and B.S. Aeronautical & Astronautical Engineering, Purdue University
- 📫 [andreagoh0101@gmail.com](mailto:andreagoh0101@gmail.com) · [LinkedIn](https://linkedin.com/in/goh-andrea)

---

### Featured: [ai-portfolio](https://github.com/andreag0101/ai-portfolio)

**[Live demo →](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/)**

10 interactive computer vision demos, 8 deep learning projects, and a retrieval-augmented research assistant — each implemented from first principles (hand-rolled Harris corners, RANSAC, PCA/LDA, backpropagation, TF-IDF retrieval) rather than a wrapped library call, with a live demo, a write-up, and tests behind it. Every demo bundles a precomputed sample so it works even if the backend is asleep; the repo has a pytest suite and CI (badge on the repo) covering the retrieval pipeline specifically, since that's the part most likely to silently regress.

<table>
<tr>
<td width="200"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/panorama"><img width="200" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/thumbnails/panorama.jpg" /></a></td>
<td width="200"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/research-assistant"><img width="200" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/thumbnails/research-assistant.jpg" /></a></td>
<td width="200"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/object-detection"><img width="200" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/deep-learning/object-detection/detections-strip.jpg" /></a></td>
<td width="200"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/gan-diffusion"><img width="200" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/deep-learning/gan-diffusion/gan-faces-wide.png" /></a></td>
</tr>
<tr>
<td><b>Panorama Stitcher</b><br/>SIFT + from-scratch RANSAC + Levenberg-Marquardt</td>
<td><b>Research Assistant (RAG)</b><br/>Hand-rolled TF-IDF retrieval, Claude-generated cited answers</td>
<td><b>Object Detection from Scratch</b><br/>Custom anchor boxes, YOLO-style loss, curated COCO subset</td>
<td><b>GANs vs. Diffusion</b><br/>DCGAN from scratch vs. pretrained diffusion, scored by FID</td>
</tr>
</table>

<details>
<summary><b>All 19 projects, by category</b></summary>

#### Computer vision — Geometric Vision

<table>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/projective-geometry"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/thumbnails/projective-geometry.jpg" /></a></td>
<td>

**[Projective Geometry Playground](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/projective-geometry)**
Homogeneous points and lines, duality, and line intersection with cross products.
</td>
</tr>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/homography"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/thumbnails/planar-rectification.jpg" /></a></td>
<td>

**[Planar Rectification & Compositing](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/homography)**
Automatic quadrilateral detection + a 4-point DLT homography to straighten a photo or warp an image into it.
</td>
</tr>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/calibration"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/thumbnails/camera-calibration.jpg" /></a></td>
<td>

**[Camera Calibration](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/calibration)**
Zhang's method: from-scratch corner detection, homographies, closed-form intrinsics, Levenberg-Marquardt refinement.
</td>
</tr>
</table>

#### Computer vision — Features, Matching & Stitching

<table>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/corners"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/thumbnails/corner-matching.jpg" /></a></td>
<td>

**[Corner Detection & Feature Matching](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/corners)**
From-scratch multiscale Harris corners matched across image pairs with SSD and NCC.
</td>
</tr>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/panorama"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/thumbnails/panorama.jpg" /></a></td>
<td>

**[Panorama Stitcher](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/panorama)**
SIFT correspondences, a custom RANSAC, and Levenberg-Marquardt refinement stitched into one image.
</td>
</tr>
</table>

#### Computer vision — Segmentation & Texture

<table>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/segmentation"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/thumbnails/image-segmentation.jpg" /></a></td>
<td>

**[Interactive Image Segmentation](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/segmentation)**
Iterative Otsu thresholding (color and texture) with morphological cleanup and contour extraction.
</td>
</tr>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/texture"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/thumbnails/texture-classification.jpg" /></a></td>
<td>

**[Texture-Based Scene Classification](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/texture)**
Rotation-invariant Local Binary Patterns and Gram-matrix style features for weather classification.
</td>
</tr>
</table>

#### Computer vision — Stereo & 3D

<table>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/disparity"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/thumbnails/stereo-disparity.jpg" /></a></td>
<td>

**[Dense Stereo Depth Estimation](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/disparity)**
Epipolar geometry and a census-transform windowed dense disparity map, unprojected into a live 3D point cloud.
</td>
</tr>
</table>

#### Computer vision — Recognition & Detection

<table>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/face"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/thumbnails/face-recognition.jpg" /></a></td>
<td>

**[Face Recognition: Eigenfaces vs. Fisherfaces](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/face)**
PCA and Fisher-LDA subspace projections, nearest-neighbor matched against 30 people.
</td>
</tr>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/car-detection"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/thumbnails/car-detection.jpg" /></a></td>
<td>

**[Car Detection: Haar Features + AdaBoost](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/car-detection)**
Integral-image Haar-like features boosted with AdaBoost, Viola-Jones style.
</td>
</tr>
</table>

#### Deep learning — From-Scratch Foundations

<table>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/fundamentals"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/deep-learning/fundamentals/custom-dataset-samples.png" /></a></td>
<td>

**[PyTorch Data Pipelines & Python Foundations](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/fundamentals)**
Python's iterator protocol, a custom Dataset/DataLoader, and a parallel-loading benchmark (34× speedup).
</td>
</tr>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/backprop-optimizers"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/deep-learning/backprop-optimizers/multi-neuron-optimizers.png" /></a></td>
<td>

**[Backpropagation & Optimizers, From Scratch](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/backprop-optimizers)**
Hand-derived forward/backward passes and SGD / SGD+Momentum / Adam, raced against torch.autograd.
</td>
</tr>
</table>

#### Deep learning — Convolutional Networks

<table>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/cnn-dataset-design"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/deep-learning/cnn-dataset-design/dataset-grid.jpg" /></a></td>
<td>

**[Custom CNN Classifier & Dataset Design](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/cnn-dataset-design)**
Three self-assembled COCO subsets isolate how dataset composition, not architecture, drives accuracy.
</td>
</tr>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/cnn-architecture-ablations"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/deep-learning/cnn-architecture-ablations/net3-confusion.png" /></a></td>
<td>

**[CNN Architecture Ablations](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/cnn-architecture-ablations)**
Depth (2 → 3 → 8 conv layers) and skip-connection downsampling strategy, isolated on CIFAR-10.
</td>
</tr>
</table>

#### Deep learning — Detection & Segmentation

<table>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/object-detection"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/deep-learning/object-detection/detections-strip.jpg" /></a></td>
<td>

**[Object Detection From Scratch on COCO](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/object-detection)**
5 anchor aspect ratios over an 8×8 grid; a combined objectness + bbox + classification loss.
</td>
</tr>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/semantic-segmentation"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/deep-learning/semantic-segmentation/mask-grid.png" /></a></td>
<td>

**[Semantic Segmentation: mUNet + ASPP](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/semantic-segmentation)**
A multi-channel U-Net plus Atrous Spatial Pyramid Pooling and a tuned Dice-loss weight.
</td>
</tr>
</table>

#### Deep learning — Generative Models

<table>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/gan-diffusion"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/deep-learning/gan-diffusion/gan-faces-wide.png" /></a></td>
<td>

**[GANs vs. Diffusion: Face Generation](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/gan-diffusion)**
A DCGAN trained from scratch on CelebA, benchmarked against a pretrained diffusion model by FID.
</td>
</tr>
</table>

#### Deep learning — Sequence Models

<table>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/transformer-translation"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/deep-learning/transformer-translation/fg-loss.png" /></a></td>
<td>

**[Transformer Machine Translation: Post-LN vs. Pre-LN](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/transformer-translation)**
Two Transformer variants trained as English→Spanish translators, scored by Levenshtein edit distance.
</td>
</tr>
</table>

#### AI Engineering

<table>
<tr>
<td width="160"><a href="https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/research-assistant"><img width="160" src="https://raw.githubusercontent.com/andreag0101/ai-portfolio/main/frontend/public/thumbnails/research-assistant.jpg" /></a></td>
<td>

**[Research Assistant (RAG)](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/research-assistant)**
From-scratch TF-IDF retrieval (no vector DB) over 555 indexed chunks, Claude-generated cited answers, with a [model card](https://github.com/andreag0101/ai-portfolio/blob/main/backend/app/rag/MODEL_CARD.md).
</td>
</tr>
</table>

</details>

---

### Tech I use

`Python` `PyTorch` `FastAPI` `TypeScript` `React` `OpenCV` `scikit-learn` `Docker` `AWS Bedrock` `Claude API`
