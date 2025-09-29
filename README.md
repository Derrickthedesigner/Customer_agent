# MULTIMODAL CUSTOMER AGENT.

A multimodal customer support assistant built with Gradio, Groq's Moonshot LLM, BLIP image captioning, and Tesseract OCR. This project enables users to submit text and/or images and receive concise, context-aware replies powered by AI — with escalation logic, confidence scoring, and visual analysis.

---

## Features

-  **OCR Integration**  
  Extracts readable text from uploaded images using Tesseract OCR (`pytesseract`), enabling support for scanned documents, receipts, and handwritten notes.

-  **BLIP Image Captioning**  
  Uses Salesforce’s BLIP model to generate descriptive captions for uploaded images, enhancing context for visual queries.

-  **Groq LLM Support**  
  Integrates Groq’s Moonshot Kimi-K2 model to generate fast, accurate responses based on user input and image-derived context.

-  **Confidence Estimation**  
  Evaluates the certainty of each LLM response using keyword heuristics and tone analysis to flag low-confidence replies.

-  **Escalation Logic**  
  Automatically detects escalation-worthy queries (e.g. refund, complaint, legal) and routes them to human agents when needed.

-  **Gradio Chat Interface**  
  Clean, interactive UI for real-time chat, image upload, and metadata display — ideal for customer-facing deployments.

---

##  Installation

Install required packages:

```bash
pip install groq gradio pillow pytesseract transformers accelerate torch torchvision timm
