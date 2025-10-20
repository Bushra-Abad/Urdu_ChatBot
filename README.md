🗣️ Urdu Conversational Chatbot: Transformer with Multi-Head Attention
📘 Overview

This project implements a custom Urdu conversational chatbot built from scratch using the Transformer Encoder–Decoder architecture with Multi-Head Attention.
The chatbot is designed to understand Urdu text, capture contextual meaning, and generate natural, fluent responses in Urdu.

A Streamlit/Gradio interface enables real-time chatbot interaction with users, supporting Urdu right-to-left text rendering.

🎯 Objectives

Develop an Urdu chatbot without using pre-trained models.

Implement a Transformer architecture from scratch using PyTorch.

Utilize Multi-Head Attention to capture deep contextual relationships.

Build an interactive Streamlit/Gradio UI for real-time chat.

Evaluate the model using both automatic and human metrics.

📊 Dataset

The model is trained on the publicly available Urdu Conversational Dataset:
📎 Kaggle – Urdu Dataset 20,000

Language: Urdu

Type: Dialogue-based text dataset

Split:

Train: 80%

Validation: 10%

Test: 10%

⚙️ Project Workflow
1️⃣ Data Preprocessing

Normalize Urdu text (remove diacritics, standardize Alef & Yeh forms).

Tokenize sentences and construct a vocabulary.

Prepare dataset splits for training, validation, and testing.

2️⃣ Model Architecture

Built entirely from scratch in PyTorch, featuring:

Encoder–Decoder structure

Multi-Head Attention mechanism

Positional Encoding

Feed-Forward Networks

3️⃣ Training & Hyperparameters
Parameter	Suggested Values
Embedding Dimension	256 / 512
Attention Heads	2
Encoder Layers	2
Decoder Layers	2
Dropout	0.1 – 0.3
Batch Size	32 / 64
Learning Rate	1e-4 – 5e-4 (Adam Optimizer)

Teacher forcing used during training

Best model saved based on Validation BLEU score

4️⃣ Evaluation

Automatic Metrics: BLEU, ROUGE-L, chrF, Perplexity
Human Evaluation: Fluency, Relevance, Adequacy (1–5 scale)
Qualitative analysis includes chatbot responses vs. ground truth comparisons.

5️⃣ Inference & UI

Urdu text input box

Model-generated Urdu reply display

Conversation history window

Decoding options: Greedy / Beam Search

Right-to-left text rendering support

Deployed via Streamlit Cloud or Gradio public link

🚀 Deployment

The chatbot can be run locally or deployed online.

▶️ Local Run
pip install -r requirements.txt
python app.py

🌐 Online Demo

You can deploy using:

Streamlit Cloud: streamlit.io/cloud

Gradio Share Link: via gr.Interface.launch(share=True)

🧪 Deliverables

✅ Full GitHub Repository (Code + Documentation)

✅ Deployed Chatbot Interface

✅ Evaluation Report

✅ Medium Blog Post (dataset, model, and demo link)
