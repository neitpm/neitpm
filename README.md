# Pham Minh Tien

**AI / Deep Learning Engineer**  
📍 Ho Chi Minh City, Vietnam · ✉️ [neit.pm.work@gmail.com](mailto:neit.pm.work@gmail.com) · 🌐 [GitHub](https://github.com/neitpm) · 🤗 [Hugging Face](https://huggingface.co/neitpm)

---

### Professional Summary

AI Engineer specializing in **Computer Vision**, **Document AI / OCR**, and **Multi-Horizon Time-Series Forecasting**. Experienced in designing deep neural architectures (KAN, Transformers, CNNs, Bi-directional Recurrence), building reproducible CPU/edge inference pipelines (ONNX Runtime), and publishing verified model packages to the Hugging Face Hub. Focused on empirical benchmarking, numerical parity validation, and end-to-end full-stack AI deployment.

---

### Technical Skills

- **Core AI & Deep Learning:** Computer Vision, Document Layout Analysis, Object Detection, Biometric ROI Localization, Multi-Horizon Time-Series Forecasting, Quantile Loss Modeling.
- **Generative AI & NLP:** LLM Orchestration, Retrieval-Augmented Generation (RAG), Vector Databases (pgvector), Hybrid Search (BM25 + Semantic), Cross-Encoder Reranking, Prompt Engineering.
- **Frameworks & Modeling:** PyTorch, TorchVision, Ultralytics YOLO, Albumentations, OpenCV, pycocotools, Hugging Face Hub.
- **MLOps & Edge Deployment:** ONNX, ONNX Runtime, Numerical Parity Verification, Model Versioning, SHA-256 Checksums, Docker Compose, Git.
- **Backend & Data Engineering:** Python, FastAPI, Flask, Streamlit, PostgreSQL, NumPy, Pandas, scikit-learn.

---

### Featured AI & Machine Learning Projects

#### 🛢️ [Multi-Horizon Oil Price Forecasting System](https://github.com/neitpm/Hybridtrinet_Oil)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)](https://github.com/neitpm/Hybridtrinet_Oil) [![Hugging Face](https://img.shields.io/badge/Hugging%20Face-Model%20Bundle-orange?logo=huggingface)](https://huggingface.co/neitpm/hybridtrinet-oil-forecasting)  
*Python, PyTorch, NumPy, Pandas, scikit-learn, PostgreSQL, Streamlit, Plotly, Docker Compose, Hugging Face Hub*
- Implemented **GUMNet**, a probabilistic quantile forecaster combining Wavelet-KAN, dilated CNN, and GRU-attention branches with adaptive gating; also developed **HybridTriNet** with RBF-KAN, GRU, and Patch Transformer branches.
- Built a multi-horizon training and evaluation pipeline for 1-, 5-, 10-, 15-, 20-, 30-, and 60-step forecasts using chronological splits, train-only scaling, and separated target windows. On a single rolling-origin holdout covering seven forecast horizons, GUMNet achieved a mean MAE of 8.19 in the dataset's original price units and MAPE of 7.02%.
- Packaged a clean 15-feature HybridTriNet release with independent inference code, per-horizon checkpoints, scalers, metadata, SHA-256 checksums, deterministic verification, and reproducible CPU inference.
- Published versioned checkpoints and reproducible inference resources on Hugging Face Hub, with architecture and input-contract documentation maintained in the GitHub README.

#### 🖐️ [Palm-Vein ROI Detection Benchmark & Recognition Prototype](https://github.com/neitpm/Palm-Vein-Recognition-Benchmark)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)](https://github.com/neitpm/Palm-Vein-Recognition-Benchmark) [![Hugging Face](https://img.shields.io/badge/Hugging%20Face-Model%20Weights-orange?logo=huggingface)](https://huggingface.co/neitpm/ssdlite-palm-vein-roi)  
*Python, PyTorch, TorchVision, OpenCV, ONNX Runtime, pycocotools, Albumentations, Hugging Face Hub*
- Built a COCO-based benchmark comparing **SSDLite-MobileNetV3** and **Faster R-CNN** for palm ROI localization on a shared validation split; historical artifacts reported 0.669–0.685 mAP@[0.5:0.95].
- Developed a CPU-based ONNX inference prototype with image preprocessing, in-graph detection postprocessing, ROI coordinate scaling, and checkpoint integrity verification.
- Exported SSDLite-MobileNetV3 to ONNX with Opset 14 and verified numerical parity against the PyTorch reference on sampled repository images using one-to-one greedy IoU matching.
- Published versioned model artifacts and inference resources on Hugging Face Hub, with architecture, latency benchmarks, and evaluation scripts documented in the GitHub README.

#### 📄 [BE-OCR Core: Document Layout Analysis & Reconstruction Pipeline](https://github.com/neitpm/be-ocr-core)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)](https://github.com/neitpm/be-ocr-core)  
*Python, OpenCV, PP-Structure, PyMuPDF, Flask, Streamlit, Docker*
- Engineered an end-to-end OCR and layout analysis pipeline converting scanned administrative PDFs and images into structured Microsoft Word (`.docx`) documents with high geometric fidelity.
- Developed an `AdaptiveTableExtractor` utilizing morphological grid analysis to isolate nested border and borderless table structures.
- Implemented automated deskewing (Hough transform), 90°/270° orientation correction, and heuristic post-processing for seals, signatures, and Vietnamese typography.
- Designed a unified document processing engine shared between an interactive Streamlit evaluation dashboard and a secure Flask REST API with token authentication and rate-limiting.

#### 🔍 [ProjectLens: Enterprise Multimodal RAG Assistant](https://github.com/neitpm/titsmart-rag)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)](https://github.com/neitpm/titsmart-rag)  
*Python, PostgreSQL (pgvector), Sentence-Transformers, BM25, Cross-Encoder, Ollama, Streamlit*
- Built a domain-adapted RAG system enabling semantic search and question answering across heterogeneous project documents (PDF, DOCX, XLSX, drawings, and images).
- Implemented a hybrid retrieval engine combining vector similarity search (Sentence-Transformers + pgvector) and lexical search (in-memory BM25) reranked via a neural Cross-Encoder.
- Integrated deterministic query routing for structured metadata lookups (e.g. project cost and technical specs) and grounded LLM synthesis with strict citation traceability.

#### 🚦 [Trafic: Vietnamese Traffic Sign Localization with Custom YOLO11n-UIB](https://github.com/neitpm/Trafic)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)](https://github.com/neitpm/Trafic)  
*Python, PyTorch, Ultralytics YOLO, OpenCV, Streamlit, Plotly*
- Conducted architectural exploration on Vietnamese traffic sign detection (VRTSD 58 categories) by integrating **Universal Inverted Bottleneck (UIB)** blocks with depthwise separable convolutions into YOLO11n.
- Designed a 4-scale detection topology (P2–P5) with a dedicated high-resolution P2 head to address high-density small-sign detection challenges in complex urban clutter.
- Evaluated parameter scaling, computational complexity (GFLOPs), and inference latency profiles across standard and inverted bottleneck configurations.

---

### Connect & Verify
- 💻 **GitHub:** [@neitpm](https://github.com/neitpm)
- 🤗 **Hugging Face:** [@neitpm](https://huggingface.co/neitpm)
- ✉️ **Email:** [neit.pm.work@gmail.com](mailto:neit.pm.work@gmail.com)
