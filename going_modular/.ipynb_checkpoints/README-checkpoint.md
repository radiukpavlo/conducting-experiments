# Going Modular Scripts

The Python scripts in this directory were generated using the notebook [05. Going Modular Part 2 (script mode)](https://colab.research.google.com/github/radiukpavlo/applied-math-packages/blob/main/01_notebooks/amp_05_pytorch_going_modular_script_mode.ipynb).

They breakdown as follows: 
* `data_setup.py` - a file to prepare and download data if needed.
* `engine.py` - a file containing various training functions.
* `model_builder.py` - a file to create a PyTorch TinyVGG model.
* `train.py` - a file to leverage all other files and train a target PyTorch model.
* `utils.py` - a file dedicated to helpful utility functions.
* **Extra:** `predictions.py` - a file for making predictions with a trained PyTorch model and input image.

For an explanation of how this was done, refer to section [05. PyTorch Going Modular of the learnpytorch.io book](https://github.com/radiukpavlo/applied-math-packages/tree/main/going_modular).