# AI Interactive Studio: Gradio & Hugging Face Tutorial

This repository contains a comprehensive tutorial on building interactive machine learning applications using **Gradio** and **Hugging Face Transformers**. The tutorial is designed to take you from layout fundamentals to deploying a multi-model AI studio in a single notebook.

## Tutorial Overview
The tutorial is structured into two main parts:
1.  **Gradio Fundamentals**: A deep dive into building custom web interfaces using `gr.Blocks()`. It covers complex layouts (Rows and Columns), handling various input types (Sliders, Dropdowns, Radios), and dynamic image generation using PIL.
2.  **AI Creative Studio**: A demonstration of integrating state-of-the-art pre-trained models. You will learn how to leverage the Hugging Face `pipeline` API to combine computer vision and natural language processing into a cohesive, tabbed application.

---

## The Applications

### 1. Mood-Based Color Palette Generator
A custom-built application that translates human emotions into aesthetic color schemes. 
* **Functionality**: Users select a mood (e.g., "Creative" or "Calm") and adjust technical parameters like temperature and saturation.
* **Logic**: The app uses the `colorsys` library to manipulate HSV color spaces and generates a high-resolution palette image with HEX and RGB labels.

### 2. AI Creative Studio
A multi-modal AI dashboard featuring three distinct powerful models:

| Feature | Hugging Face Model | Description |
| :--- | :--- | :--- |
| **Sentiment Analyzer** | `distilbert-base-uncased-finetuned-sst-2-english` | A fast, light-weight transformer that classifies the emotional tone of text as Positive or Negative. |
| **Image Storyteller** | `Salesforce/blip-image-captioning-base` | A Bootstrapping Language-Image Pre-training (BLIP) model that understands image content to generate captions. |
| **Creative Writer** | `gpt2` | A generative model used to extend captions into full stories or continue user-provided prompts. |

---

## Installation & Setup

To run the notebook locally or in Google Colab, you will need the following dependencies:

```python
!pip install gradio transformers torch pillow
