# Fine-tuned LLAMA-3.2-1b Model for Mental Health Conversations

This repository contains a fine-tuned version of the LLAMA-3.2-1b model on a mental health counseling dataset. The model is designed to generate empathetic, context-aware responses suitable for mental health support and counseling tasks.

---

## Model Overview
- **Base Model**: ["meta-llama/Llama-3.2-1B"](https://huggingface.co/meta-llama/Llama-3.2-1B)
- **Dataset**: Fine-tuned on a curated mental health dataset (["marmikpandya/mental-health"](https://huggingface.co/datasets/marmikpandya/mental-health))
- **Objective**: Improve the model's ability to generate empathetic, coherent, and contextually appropriate responses in mental health counseling scenarios.
- **Training Hardware**: Trained using an NVIDIA Tesla P100 GPU on Kaggle.

#### Training Configuration

The fine-tuned model was trained with the following configuration:

- **train dataset size**: 10,680 
- **Epochs**: 1  
- **Batch Size**: 1  
- **Learning Rate**: 3e-5  
- **Optimizer**: AdaFactor 

---

## Features
- Generates context-aware responses tailored to mental health conversations.
- Fine-tuned for empathy, validation, and supportive language.
- Suitable for applications in mental health chatbots and support systems.

---

## Usage

### Access the Model
The Python Notebook with all the code is provided in this repo. The model and related files are also available on Kaggle and can be viewed and downloaded at https://www.kaggle.com/code/shussain37/llama-3-mental-health

### Compare Pretrained and Fine-tuned Model Responses

We have included a CSV file (`response_comparison.csv`) with 50 sample responses comparing the pretrained model and the fine-tuned model on questions from the test dataset. Below is an example of responses from both a pre-trained and fine-tuned model. Clearly, the fine-tuned model generates context-aware responses tailored to mental health conversations.

**Question**: I think I might have depression. What should I do?
**Pre-trained Model Response**:  I have been feeling sad, empty, and like I'm not living my life. I'm a 22 year old female and I think I might have depression. I don't know what to do. I don't want to feel this way anymore. I have been feeling sad, empty, and like I'm not living my life. I'm a 22 year old female and I think I might have depression. I don't know what to do. I don't want to feel this way anymore. I have been feeling sad
**Fine-tuned Model Response**: It's important to seek professional help if you think you may have depression. We can work together to develop a treatment plan that works for you, which may include therapy, medication, or a combination of both. It's important to remember that depression is a treatable condition, and that you don't have to go through this alone. Have you considered seeking help from a mental health professional? You don't have to go through this alone.Â https://www.mh.org/about-mh/symptoms-conditions/depression/
**Dataset Answer**: It's important to seek professional help if you think you may be experiencing depression. A licensed therapist can provide you with a proper diagnosis and recommend appropriate treatment options, such as therapy or medication.
