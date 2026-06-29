# Multi-Modal Chest X-Ray Intelligence System

A multimodal medical AI system that combines Retrieval-Augmented Generation (RAG), Vision-Language Models (VLMs), and vector search to support clinical question answering and automated radiology report generation from chest X-ray images.

---

## Project Overview

This project implements an end-to-end medical vision-language pipeline capable of:

* Answering clinical questions about chest X-rays using multimodal retrieval.
* Automatically generating preliminary radiology reports from uploaded X-ray images.
* Comparing different visual retrieval models for medical image search.

The system integrates multiple state-of-the-art AI models into a unified Gradio interface designed for medical image understanding.

---

## Features

* Multi-modal Retrieval-Augmented Generation (RAG)
* Clinical Question Answering
* Automated Radiology Report Generation
* Chest X-ray Image Retrieval
* Medical Vision-Language Understanding
* Comparative Evaluation of CLIP and ColPali
* Interactive Gradio Web Interface
* Quantized Large Vision-Language Models

---

## System Architecture

The project consists of two independent pipelines:

### Clinical QA Pipeline

* User submits a clinical question.
* Chest X-ray images are indexed using multiple retrieval models.
* The most relevant image is retrieved.
* Retrieved evidence and user query are passed to MedGemma.
* Grounded clinical response is generated.

### Report Generation Pipeline

* User uploads a Chest X-ray.
* MedGemma analyzes the image.
* A structured preliminary radiology report is generated automatically.

---

## AI Models

### Vision Retrieval

* ColPali (Late Interaction Retrieval)
* OpenAI CLIP

### Vision-Language Generation

* Google MedGemma-4B-IT

### Vector Database

* Qdrant

---

## Technologies

* Python
* PyTorch
* Hugging Face Transformers
* MedGemma
* CLIP
* ColPali
* Qdrant
* Gradio
* BitsAndBytes
* Retrieval-Augmented Generation (RAG)

---

## Results

The project demonstrated that:

* CLIP achieved superior retrieval performance for chest X-ray semantic search.
* MedGemma successfully generated clinically structured radiology reports.
* ColPali highlighted the limitations of document-oriented retrieval models when applied directly to medical imaging without domain-specific fine-tuning.

---

## Learning Outcomes

* Vision-Language Models (VLMs)
* Medical AI
* Retrieval-Augmented Generation
* Vector Databases
* Clinical Image Retrieval
* Large Language Models
* Medical Report Generation
* Multimodal Deep Learning

---

## Future Improvements

* Fine-tune retrieval models on medical imaging datasets.
* Support additional imaging modalities (CT and MRI).
* Deploy using scalable cloud infrastructure.
* Improve report evaluation with clinical metrics.

---

## Author

**Zeyad Sherif**
