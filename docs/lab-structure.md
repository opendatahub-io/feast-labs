## Lab Structure

Each domain-specific lab includes the following key components:

### 1\. Data Sources

This section contains raw data relevant to the specific domain.

  * **Raw Data:** Example datasets in formats such as CSV, JSON, or SQL database dumps.
  * **Data Generation Scripts (Optional):** Scripts to generate synthetic data if real-world data is sensitive or too large.

### 2\. Feast Feature Store Setup

This component focuses on defining and managing features using Feast.

  * **Feast Project Initialization:** Instructions and scripts to initialize a Feast project within the lab's directory.
  * **Feature Definitions:** Python files containing `FeatureView` and `Entity` definitions.
  * **Offline Store Configuration:** Configuration for offline stores (e.g., Parquet files, BigQuery).
  * **Online Store Configuration:** Configuration for online stores (e.g., Redis, DynamoDB).

### 3\. Data Ingestion & Feature Materialization

This part details the process of loading raw data into the Feast Feature Store.

  * **Ingestion Scripts:** Python scripts to read raw data and ingest it into the Feast offline/online store.
  * **Materialization:** Instructions and scripts to materialize historical features for training.

### 4\. Feature Serving for Model & Inference

This section covers how features are retrieved for model training and online inference.

  * **Feature Retrieval for Training:** Example code demonstrating how to retrieve historical features for training machine learning models.
  * **Online Feature Retrieval:** Example code demonstrating how to retrieve online features for real-time inference.

### 5\. Prototype Streamlit Application

A small prototype Streamlit application is included to showcase the inference process.

  * **User Interface:** A simple UI for users to interact with.
  * **Chatbot-like Interaction:** The application simulates a chatbot interaction where user input triggers feature retrieval and model inference.
  * **Inference Display:** The application displays the model's prediction or output based on the retrieved features.
  * **Dependency Management:** A `requirements.txt` file listing all necessary Python packages.



## Items Checklist

The following is a checklist of required items for each lab, moving from raw data to model inference:

| Item Type                     | Description                                                             | Responsibility | Status        |
| :---------------------------- | :---------------------------------------------------------------------- | :------------- | :------------ |
| **Raw Data Source**           | Sample dataset(s) specific to the domain.                               | Person         | To be created |
| **Feast Feature Definitions** | `feature_store.yaml`, `definitions.py` with entities and feature views. | Person         | In progress   |
| **Model Code (Optional)**     | Simple ML model demonstrating feature consumption.                      | Person         | To be created |
| **Streamlit App**             | `app.py` for inference demonstration.                                   | Person         | To be created |
| **requirements.txt**          | List of all Python dependencies.                                        | Person         | To be created |
| **Lab README**                | Detailed instructions for setting up and running the lab.               | Person         | To be created |

