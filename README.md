A multimodal AI pipeline that converts an image into a caption, expands it into a creative story, and converts the story into speech audio.

🚀 Project Overview

This project integrates Computer Vision + NLP + Text-to-Speech using pre-trained models.

Pipeline
BLIP → Generates a caption from the input image
FLAN-T5 → Converts the caption into a story
gTTS → Converts the story into an audio file
Gradio UI → Simple interactive interface

📦 Models Used
BLIP (Salesforce/blip-image-captioning-base) - Pre-trained on large image–text datasets (like COCO)
FLAN-T5 Small (google/flan-t5-small) - Pre-trained on instruction-tuning datasets
gTTS for Text-to-Speech

🧠 Why No Training?
Training BLIP or T5 requires high-end GPUs and extremely large datasets.
So we used pre-trained models and focused on building a full working pipeline.

💻 Tech Stack
Python
Transformers (Hugging Face)
PyTorch
Gradio
gTTS
PIL

▶️ How to Run
pip install transformers torch gTTS gradio pillow
python app.py

Upload an image → get caption → generate story → listen to audio.

🎯 Features
End-to-end working multimodal pipeline
Uses state-of-the-art pretrained models
Works on CPU (no GPU needed)

👩‍🏫 Use Case
Perfect for academic demonstration of:
Vision + Language models
Pretrained ML usage
End-to-end AI application integration

