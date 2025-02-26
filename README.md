# AI Powered IVR Prototype Leveraging LLM for Customer Service

# IVR System Powered by LLM

This repository contains a IVR (Interactive Voice Response) system prototype powered by the LLM. The project demonstrates an end-to-end workflow that:
- Transcribes user audio input,
- Processes the text using the Falcon language model,
- Generates a response, and
- Converts that response back into speech.

The system is designed to run in a Python environment, making it easy to prototype and test conversational interactions in an online business context.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Demo Scenario](#demo-scenario)
- [Architecture](#architecture)


## Overview

This project serves as a prototype IVR system for online business applications, think customer service for platforms like Amazon, Ebay or similar. For example, when asked, "Are there any special deals or discounts on electronics today?", the system produced the following response:

- 1.6 GHz Intel Core i5-3210M  
- 4 GB RAM  
- 500 GB HDD  
- 15.6" HD LED display  
- Intel HD Graphics 4000  
- DVD-RW


## Features

- **Speech-to-Text:** Converts uploaded audio (WAV files recommended) into text using Google's Speech Recognition API.
- **Language Generation:** Uses Falcon LLM to generate responses from transcribed text.
- **Text-to-Speech:** Converts the generated text response into speech via the gTTS library.
- **Google Colab Integration:** A single notebook brings together all steps, facilitating rapid prototyping and testing.

## Demo Scenario

For demonstration, consider the following customer query:
> **Customer:** "Are there any special deals or discounts on electronics today?"

The LLM processed this query and returned a list of hardware specifications:
- 1.6 GHz Intel Core i5-3210M  
- 4 GB RAM  
- 500 GB HDD  
- 15.6" HD LED display  
- Intel HD Graphics 4000  
- DVD-RW  

The response illustrates the system’s capability to generate structured output. This response can be refined when I integrate business-specific data (such as Amazon, Ebay or similar) and adjusting the prompt engineering.

## Architecture

The project is organized into the following components:

1. **Audio Upload & Transcription:**  
   Users upload a `.wav` file that is transcribed into text using the SpeechRecognition library.

2. **Language Processing:**  
   The transcribed text is fed into the LLM, which generates a contextual response.

3. **Audio Synthesis:**  
   The generated text is converted to speech using gTTS and played back within the notebook.

4. **Integration:**  
   All components are orchestrated within a notebook for seamless interaction.


