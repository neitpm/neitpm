<div align="center">

# Pham Minh Tien
### AI Engineer

[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-neitpm-orange?style=flat-square)](https://huggingface.co/neitpm)
[![GitHub](https://img.shields.io/badge/GitHub-neitpm-blue?style=flat-square&logo=github)](https://github.com/neitpm)
[![Email](https://img.shields.io/badge/Email-neit.pm.work%40gmail.com-red?style=flat-square&logo=gmail)](mailto:neit.pm.work@gmail.com)

</div>

---

### About Me

I am an **AI Engineer** specializing in Deep Learning, Computer Vision, Document AI, and Multi-Horizon Time-Series Forecasting. I focus on developing clean, reproducible model architectures, verifying numerical parity across frameworks, and packaging models for standalone inference and evaluation.

---

### What I Do & What I've Built

- **Time-Series & Commodity Forecasting:**
  - Researched and developed **GUMNet** (Wavelet-KAN + Dilated CNN + GRU-Attention with adaptive gating) and **HybridTriNet** (RBF-KAN + GRU + Patch Transformer).
  - Built multi-horizon evaluation pipelines (1, 5, 10, 15, 20, 30, 60 steps) with train-only scaling and published verified bundles on [Hugging Face](https://huggingface.co/neitpm/hybridtrinet-oil-forecasting).

- **Computer Vision & Biometrics:**
  - Benchmarked one-stage (SSDLite-MobileNetV3) vs. two-stage (Faster R-CNN) object detection for palm-vein ROI extraction on custom COCO splits.
  - Exported models to ONNX (Opset 14), verified PyTorch–ONNX numerical parity, and published CPU inference benchmarks on [Hugging Face](https://huggingface.co/neitpm/ssdlite-palm-vein-roi).
  - Explored custom Universal Inverted Bottleneck (UIB) backbones and 4-scale heads (P2–P5) on YOLO11 for Vietnamese traffic sign localization.

- **Document AI & Layout Analysis:**
  - Engineered end-to-end OCR and document reconstruction engines converting scanned PDFs into structured Word (`.docx`) files with table boundary extraction (`AdaptiveTableExtractor`), deskewing, and orientation correction.

- **Enterprise Retrieval-Augmented Generation (RAG):**
  - Built domain-adapted document assistants combining vector search (pgvector), lexical search (BM25), and Cross-Encoder neural reranking with locally served LLMs.

---

### Core Technologies

- **Frameworks & Modeling:** PyTorch, TorchVision, Ultralytics YOLO, Transformers, KAN.
- **Vision & Layout:** OpenCV, Albumentations, PP-Structure, PyMuPDF, pycocotools.
- **Inference & MLOps:** ONNX Runtime, Hugging Face Hub, Docker Compose, Git.
- **Data & Backend:** Python, FastAPI, Flask, Streamlit, PostgreSQL (pgvector), NumPy, Pandas.

---

<div align="center">
  <sub>Get in touch: <a href="mailto:neit.pm.work@gmail.com">neit.pm.work@gmail.com</a> · Hugging Face: <a href="https://huggingface.co/neitpm">@neitpm</a></sub>
</div>
