# CESNET Traffic Classification Examples 
A collection of Jupyter notebooks with examples of usage of the `cesnet-datazoo` and `cesnet-models` packages.

:frog: [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) [![](https://img.shields.io/pypi/v/cesnet-datazoo)](https://pypi.org/project/cesnet-datazoo/) [![](https://img.shields.io/badge/docs-cesnet--datazoo-blue.svg)](https://cesnet.github.io/cesnet-datazoo/)
<br/>
:brain: [CESNET Models](https://github.com/CESNET/cesnet-models)&nbsp;&nbsp;&nbsp;[![](https://img.shields.io/pypi/v/cesnet-models)](https://pypi.org/project/cesnet-models/) [![](https://img.shields.io/badge/docs-cesnet--models-blue.svg)](https://cesnet.github.io/cesnet-models/)


The following notebooks are available:

- `explore_data.ipynb` - Simple initialization of a dataset class to explore available features.
- `example_evaluation.ipynb` - Training of a LightGBM classifier and its evaluation on a per-week and per-day basis.
- `reproduce_tls.ipynb` - Use a pre-trained model from the `cesnet-models` package to reproduce the results of the *"Fine-grained TLS services classification with reject option"* paper.
- `reproduce_quic.ipynb` - Use a pre-trained model from the `cesnet-models` package to reproduce the results of the *"Encrypted traffic classification: the QUIC case"* paper.
- `example_train_nn.ipynb` - Training of a neural network from scratch. The `cesnet-datazoo` package provides a dataset, which is split into the train, validation, and test sets. The `cesnet-models` package provides the neural network architecture and data transformations.
- `month_evaluation_cesnet_tls_year22.ipynb` - Training and per-month evaluation of a LightGBM model using the CESNET-TLS-Year22 dataset.
- `cross_dataset_embedding_function.ipynb` - Multi-dataset evaluation of an embedding function designed to generalize across traffic classification tasks. A pre-trained model is obtained from the `cesnet-datazoo` package, and datasets are loaded from `tcbench` and `cesnet-datazoo` packages.

### Requirements
The dependencies are installed in the first cell of each notebook. Alternatively, the `requirements.txt` file is also provided. PyTorch with CUDA 11.8 support should be installed with the following command (more info [here](https://pytorch.org/get-started/locally/)):

```bash
python -m pip install torch>=1.10 --index-url https://download.pytorch.org/whl/cu124
```