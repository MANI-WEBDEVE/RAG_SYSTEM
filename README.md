# RAG System - Document Chunking and Data Ingestion

This repository contains Jupyter notebooks for implementing Retrieval-Augmented Generation (RAG) systems with various document chunking strategies and data ingestion pipelines.
 
### 1. RAG_CHUNK_CONCEPT.ipynb
Comprehensive guide to implementing **five different chunking methods** for RAG systems:

- **Fixed Size Chunking** - Split documents into uniform chunks
- **Semantic Chunking** - Group text by meaning and context
- **Structural Chunking** - Respect document structure (headings, sections)
- **Recursive Chunking** - Hierarchical splitting approach
- **LLM-based Chunking** - Use language models for intelligent chunking

#### Features:
- PDF document download and text extraction using PyMuPDF
- Text formatting and cleaning utilities
- Multiple chunking strategy implementations
- Compatible with Google Colab (GPU support)

#### Dependencies:
- PyMuPDF (PDF processing)
- sentence-transformers (embeddings)
- transformers
- PyTorch (CUDA support)
- accelerate, bitsandbytes, flash-attn (optimization)

### 2. RAG_Data_Ingestion.ipynb
Data ingestion pipeline for RAG systems (Note: Contains merge conflicts that need resolution)

## Quick Start

### Google Colab
Open the notebooks directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MANI-WEBDEVE/RAG_SYSTEM/blob/main/RAG_CHUNK_CONCEPT.ipynb)

### Local Installation

```bash
# Install dependencies
pip install PyMuPDF
pip install sentence-transformers
pip install tqdm
pip install accelerate
pip install bitsandbytes
pip install flash-attn --no-build-isolation

# For PyTorch with CUDA 12.1 support
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
pip install -U transformers sentence-transformers
```

## 📖 Usage

1. **Download Documents**: The notebook automatically downloads sample ML textbooks if not present
2. **Extract Text**: PDF text extraction page-by-page using PyMuPDF
3. **Apply Chunking**: Choose from 5 chunking strategies based on your use case
4. **Generate Embeddings**: Use sentence-transformers for vector representations

## 🛠️ Requirements

- Python 3.8+
- GPU recommended for embedding generation (Colab T4 supported)
- CUDA 12.1+ for GPU acceleration

## 📄 License

MIT License

## 🤝 Contributing

Feel free to open issues or submit pull requests for improvements.
