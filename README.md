# CESNET Traffic Classification Examples 
Collection of Jupyter notebooks with example usage of the `cesnet_datazoo` and `cesnet_models` packages.

- [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) [![](https://img.shields.io/pypi/v/cesnet-datazoo)](https://pypi.org/project/cesnet-datazoo/)
- [CESNET Models](https://github.com/CESNET/cesnet-models) [![](https://img.shields.io/pypi/v/cesnet-models)](https://pypi.org/project/cesnet-models/)

Currently, the following notebooks are available:

- `explore_data.ipynb` - Simple initialization of a dataset class to explore available features.
- `example_evaluation.ipynb` - Training of a LightGBM classifier and its evaluation on a per-week and per-day basis.
- `reproduce_tls.ipynb` - Use a pre-trained model from the `cesnet_models` package to reproduce the results of the *"Fine-grained TLS services classification with reject option"* paper.
- `reproduce_quic.ipynb` - Use a pre-trained model from the `cesnet_models` package to reproduce the results of the *"Encrypted traffic classification: the QUIC case"* paper.

### Requirements
The dependencies are installed in the first cell of each notebook. Alternatively, the `requirements.txt` file is also provided. PyTorch with CUDA support should be installed with the following command (more info [here](https://pytorch.org/get-started/locally/)):

```bash
python -m pip install torch>=1.10 --index-url https://download.pytorch.org/whl/cu118
```