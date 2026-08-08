# Day 01 — Understanding AI Pipelines

## Goal
Build a clear mental model of how AI systems process data, from raw input to final output, and apply that model to real-world AI products.

## The AI Pipeline

```
INPUT → PREPROCESSING → MODEL INFERENCE → POSTPROCESSING → OUTPUT
```

## Pipeline Stages

| Stage | What Happens |
|---|---|
| Input | Raw data enters the system. This can be text, an image, audio, or structured data, and it is not yet usable by a model in its original form. |
| Preprocessing | The raw input is cleaned and transformed into a numerical format, such as tokens, vectors, or pixel arrays, that the model can compute with. |
| Model Inference | The trained model processes the prepared input using its learned parameters (weights) and produces a prediction, classification, or generated result. |
| Postprocessing | The raw numerical output from the model is converted into a human-readable or usable format, such as decoded text, labels, or formatted values. |
| Output | The final result is delivered to the user or passed to another system, such as a reply, a translation, a recommendation, or a classification. |

## Real-World AI Products

| Product | Input | Processing | Output |
|---|---|---|---|
| ChatGPT | User's typed text prompt and conversation history | Text is tokenized and passed through a transformer language model, which computes probability distributions over the next token, repeated iteratively | Generated text response returned to the user |
| Google Translate | Source-language text, or speech/image converted to text via OCR | Text is tokenized and encoded by a sequence-to-sequence/transformer model, then decoded into the target language using learned cross-lingual mappings | Translated text or spoken audio in the target language |
| Spotify Recommendations | User's listening history, skip behavior, playlist data, and audio features of tracks | A recommendation model, combining collaborative filtering and content-based/embedding techniques, scores candidate tracks against user preferences and behavior patterns | Ranked list of recommended songs or playlists |

## How a Chatbot Works

A chatbot receives a user's text input and converts it into numerical tokens that the underlying language model can process. The model, trained on large volumes of text, computes a probability distribution over likely next tokens based on patterns learned during training. It generates a response by repeatedly predicting the next most probable token and appending it to the sequence. This generated sequence of tokens is then decoded back into human-readable text. The final output is displayed to the user as the chatbot's reply, with the system performing statistical pattern-based computation rather than genuine understanding or intent.

## Key Takeaway

Every AI product, regardless of how advanced it appears, follows the same underlying pipeline: structured data is prepared, a trained model computes a prediction, and that prediction is converted into a usable result. Understanding this pipeline provides a consistent framework for analyzing any AI system, from simple classifiers to large language models.

## Deliverables

- AI pipeline diagram (designed in Canva)
- Five-sentence explanation of how a chatbot works
- Documentation of three real-world AI products: ChatGPT, Google Translate, and Spotify Recommendations
