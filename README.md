# Marathi YouTube Video Summarization

## Overview

This project focuses on the development of a Natural Language Processing (NLP) model for summarizing Marathi YouTube videos. The goal is to create a system that generates a concise summary text file for a given Marathi video, providing users with a quick overview of the video's content.

## Approaches

### Approach 1: Audio-Based Summarization

In the first approach, the video is divided into a number of chunks, and the audio is extracted using the Google Speech API. Subsequently, a Hugging Face model is employed for summarization, generating a summary text file based on the recognized audio content.

### Approach 2: Language Translation for Summarization

The second approach involves the use of the Facebook BART model for summarization. Since the BART model primarily supports English, a language translation step is introduced. The Marathi text from the video is first converted to English. The BART model is then used to summarize the English text, and the resulting summary is translated back to Marathi.
