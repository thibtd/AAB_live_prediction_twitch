# Twitch Channel Message Prediction

This project uses Apache Spark to predict which Twitch channel a message belongs to, based on both historical and live chat data.

## Project Structure

-   `assignment3 - asmongold.ipynb`: A Jupyter Notebook containing the core logic for data loading, processing, model training, and evaluation using Spark.
-   `twitch_data/`: This directory holds the datasets of Twitch messages used for training and testing the prediction model.
-   `model_nlp_final/`: This directory contains the final, trained Natural Language Processing (NLP) model saved by Spark.

## Approach

The project's workflow is primarily demonstrated in the `assignment3 - asmongold.ipynb` notebook.

1.  **Data Ingestion:** Historical Twitch chat data is loaded from the `twitch_data` directory.
2.  **Model Training:** A Natural Language Processing (NLP) model is trained on this data using Spark to learn the patterns and vocabulary specific to different Twitch channels.
3.  **Model Saving:** The trained pipeline model is saved to the `model_nlp_final` directory for later use.
4.  **Prediction:** The model can be loaded to predict the origin channel for new messages, applicable to both historical logs and live data streams.
