# Super Rapid Annotator PoC

## Introduction 

The Super Rapid Annotator Proof of Concept (PoC) is a Jupyter Notebook-based application that presents a conceptual workflow for the Super Rapid Annotator system. The Super Rapid Annotator system aims to utilize a multimodal vision model and a JSON generator to annotate images/videos and output json as a response. 

## Overall Architecture

The overall system is conceptualized in two main stages: image-to-text generation using a multimodal vision model, followed by text-to-JSON structuring.

1. **Image-to-Text Generation:** Utilizing BakLlava, this stage focuses on interpreting the visual content of the image to generate descriptive annotations.
2. **Text-to-JSON Generation:** This stage involves understanding the generated text and mapping it to appropriate JSON values, facilitated by JsonFormer and additional helper functions.

## Demo

The following video demonstrates the Super Rapid Annotator PoC in action. It showcases the Gradio interface and the application's capabilities

https://github.com/A09L/Super-Rapid-Annotator-PoC/assets/73531422/80be074b-085c-440b-be32-79d74b26704a

## Getting Started

To explore the Super Rapid Annotator PoC:

1. Open the Jupyter Notebook in your preferred environment.
2. Execute the cells sequentially. The notebook will guide you through the process, from loading the image to generating annotations.
3. Upon reaching the Gradio Interface cell, the notebook will launch an interactive interface. Here, you can upload images and see the system's annotations in real time.

## TODO

* **Model Enhancement**: Develop or fine-tune a model capable of extracting relevant information from the generated text and structuring it into JSON format.
* **Model Finetuning**: Investigate additional fine-tuning or alternative models for improve accuracy in image-to-text generation.
* **Functionality Expansion**: Extend the system's capabilities to handle video inputs and extend functionality to export annotations in CSV format
* **Pipeline Optimization**: Explore the integration of LangChain for a more streamlined workflow and implement strictJSON for enhanced JSON validation.
* **User Interface**: Enhance the Gradio interface (for example make the chatbot show the image in question and make it easier to input JSON)
* **Inference Speed Optimization**: Investigate the use of smaller, more efficient models or model quantization techniques to enhance the inference speed without significantly compromising accuracy.
* **JSON Type Handling**: Enhance the system to recognize and correctly handle various JSON data types, such as integers, strings, and arrays, improving the versatility of the annotation output.
