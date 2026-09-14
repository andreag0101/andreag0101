### Hi, I'm Andrea Goh

AI/ML engineer and computer vision researcher. I like taking a system apart down to the math, rebuilding it from scratch, and shipping the result — not just calling a library and moving on.

- 🔭 Currently an **AI Development Intern at ArgonDigital**, building RAG-based LLM applications on AWS Bedrock
- 🔬 Computer Vision Research Assistant at **Purdue's Robotic Vision Lab** — multimodal transformers and 3D reconstruction pipelines built from classical vision theory, no OpenCV
- 🎓 M.S. Computer Engineering (AI/ML) and B.S. Aeronautical & Astronautical Engineering, Purdue University
- 📫 [andreagoh0101@gmail.com](mailto:andreagoh0101@gmail.com) · [LinkedIn](https://linkedin.com/in/goh-andrea)

---

### Featured: [ai-portfolio](https://github.com/andreag0101/ai-portfolio)

**[Live demo →](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/)**

11 interactive computer vision demos, 9 deep learning projects, and a retrieval-augmented research assistant — each implemented from first principles (hand-rolled Harris corners, RANSAC, PCA/LDA, backpropagation, TF-IDF retrieval) rather than a wrapped library call, with a live demo, a write-up, and tests behind it.

| Project | What's interesting about it |
|---|---|
| [Panorama Stitcher](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/panorama) | SIFT correspondences + a from-scratch RANSAC + Levenberg-Marquardt refinement |
| [Research Assistant (RAG)](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/research-assistant) | Hand-rolled TF-IDF retrieval (no vector DB) + Claude-generated, cited answers over 555 indexed chunks |
| [Object Detection from Scratch](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/object-detection) | Custom anchor boxes and a YOLO-style objectness + bbox + class loss, trained on a curated COCO subset |
| [GANs vs. Diffusion](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/deep-learning/gan-diffusion) | A DCGAN trained from scratch, benchmarked against a pretrained diffusion model by FID |
| [Camera Calibration](https://ai-portfolio-7x0t2bk8j-ai-portfolio6.vercel.app/calibration) | Zhang's method end to end: from-scratch corner detection through closed-form intrinsics to Levenberg-Marquardt refinement |

Every demo bundles a precomputed sample so it works even if the backend is asleep; the repo has a pytest suite and CI (badge on the repo) covering the retrieval pipeline specifically, since that's the part most likely to silently regress.

---

### Tech I use

`Python` `PyTorch` `FastAPI` `TypeScript` `React` `OpenCV` `scikit-learn` `Docker` `AWS Bedrock` `Claude API`
