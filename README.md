
# Automatic Speech Recognition

## Project Overview

This project implements **Automatic Speech Recognition (ASR)** using the `openai/whisper-tiny` model from Hugging Face. It transcribes audio into text using the **LibriSpeech ASR dataset**.

The repository includes:

* **Clean notebook:** `Automatic-Speech-Recognition_clean.ipynb` – ready to run.
* **Original notebook:** `Automatic_Speech_Recognition.ipynb` – includes all original examples and outputs for reference.

---

## What I Learned

* Loading and working with **streaming audio datasets**.
* Building an **ASR pipeline** using Hugging Face Transformers.
* Handling and analyzing audio data in Python (`IPython.display.Audio`).
* Comparing **model predictions vs. original transcripts**.
* Understanding audio feature extraction and transcription processes.

---

## Example Output

**Model Transcription:**

> "Chapter 16 I might have told you of the beginning of this liaison in a few lines, but I wanted you to see every step by which we came. I to agree to whatever Mark Reid wished."

**Original Transcript from Dataset:**

> "CHAPTER SIXTEEN I MIGHT HAVE TOLD YOU OF THE BEGINNING OF THIS LIAISON IN A FEW LINES BUT I WANTED YOU TO SEE EVERY STEP BY WHICH WE CAME I TO AGREE TO WHATEVER MARGUERITE WISHED"

**Observation:**
The ASR model transcribes the audio accurately, though capitalization and minor details may differ.

---

## Setup Instructions

To run this project, you need Python 3.x and the following libraries:

```bash
!pip install transformers
!pip install -U datasets
!pip install soundfile
!pip install librosa
!pip install gradio
```

Optional: Suppress warning messages from Transformers library:

```python
from transformers.utils import logging
logging.set_verbosity_error()
```

---

## How to Use

1. Open the notebook in **Google Colab** or **Jupyter Notebook**.
2. Run the notebook to explore **dataset examples, audio playback, and ASR transcriptions**.
3. Compare **model predictions** with the **original transcripts**.

**Note:** Users can download the full original notebook to see every step with examples.

---

## Notebooks in Repository

* `Automatic-Speech-Recognition_clean.ipynb` – Clean version, ready to run.
* `Automatic_Speech_Recognition.ipynb` – Full original notebook with all examples and outputs.

---



