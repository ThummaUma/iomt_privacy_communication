# iomt_privacy_communication

## Overview
This project implements a privacy-preserving federated learning pipeline for IoMT (Internet of Medical Things) data using differential privacy. The pipeline simulates a hierarchical federated setup with clients, edge servers, and a cloud server, leveraging a pre-trained autoencoder encoder and the CICIoMT2024 dataset.

## Project Structure
- `main.py.ipynb`: Main entry point. Orchestrates the federated learning pipeline.
- `client.py.ipynb`: (Stub) Intended for client-side training logic.
- `edge_server.py.ipynb`: (Stub) Intended for edge server aggregation logic.
- `cloud_server.py.ipynb`: (Stub) Intended for cloud server aggregation logic.
- `dataset.py.ipynb`: (Stub) Intended for dataset loading and splitting.
- `dp_utils.py.ipynb`: (Stub) Intended for differential privacy utilities.
- `models.py.ipynb`: (Stub) Intended for model loading utilities.
- `requirement.txt`: Python dependencies.

## Requirements
Install dependencies with:
```bash
pip install -r requirement.txt
```

## Usage
Run the main pipeline (ensure you have the required dataset and pre-trained model):
```bash
python main.py.ipynb
```

The pipeline will:
1. Load and preprocess the CICIoMT2024 dataset.
2. Distribute data among simulated clients.
3. Train local client models with differential privacy.
4. Aggregate models at edge servers.
5. Aggregate global model at the cloud server.
6. Save the final global model as `global_model.pt`.

## Notes
- The submodules (`client.py.ipynb`, `edge_server.py.ipynb`, etc.) are currently stubs and need to be implemented for full functionality.
- The main logic and workflow are in `main.py.ipynb`.
- The project is designed for research and prototyping purposes.