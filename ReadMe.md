# Text-Based Image Retrieval

## Project Overview

This project is designed to create a **text-to-image retrieval system** using advanced deep learning models. The system enables users to search for images from a dataset using natural language queries. The primary goal is to build a robust framework capable of accurately retrieving relevant images based on textual input.

## Features
- Utilizes **pretrained vision and language models** for feature extraction.
- Employs **Cosine Similarity** to rank images based on relevance to textual queries.
- Implements **Top-K Retrieval** to provide the most relevant image results.
- Supports batch processing for efficient computation.

## Datasets
The project supports the following datasets:

- MSCOCO

- Flickr30k

- Visual Genome


Ensure you download and configure the datasets properly before running the script.

## Key Components
1. **Image Encoder**: Extracts image features using a pretrained ResNet model.
2. **Text Encoder**: Converts textual queries into feature embeddings using a transformer-based model (e.g., BERT).
3. **Similarity Calculation**: Matches text and image embeddings in a shared feature space using Cosine Similarity.
4. **Inference Pipeline**: Ranks images based on their similarity to the query and retrieves the top-K results.

## Evaluation Metrics
The project evaluates the retrieval system using:

- **Cosine Similarity** for ranking.

- **Top-K Retrieval** to assess system performance.


These metrics ensure that the most relevant images appear at the top of the retrieval list.

## Requirements
- Python 3.8+
- PyTorch
- torchvision
- Transformers (HuggingFace)
- Matplotlib (optional, for visualization)

Install the dependencies using:

```
pip install -r requirements.txt
```

## How to Use
1. Clone the repository and navigate to the project directory.
2. Download and prepare the dataset as per the configuration instructions.
3. Run the notebook `script.ipynb` to train and evaluate the model.

Make sure the dataset paths and configurations are updated in the notebook.

## Example Query
To perform inference:

- Provide a natural language query like: `"A dog playing with a ball."`

- The system will return the top-K images most relevant to the query.


Example output:

```
Rank 1: <image fetched>

Rank 2: <image fetched>

Rank 3: <image fetched>

```
## Conclusion
This project demonstrates the effective integration of vision and language models for multimodal retrieval tasks. With a focus on robust evaluation and efficient processing, it lays the groundwork for scalable image retrieval systems.

Gautam Balachandran
gautam.balachandran@gmail.com