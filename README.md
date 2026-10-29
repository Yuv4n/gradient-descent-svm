# Gradient descent and linear SVM

UCL group coursework notebook: finite-difference gradient descent with plotted descent paths, then a linear SVM fitted to simulated two-dimensional data.

- **Gradient descent:** forward-difference gradients, with descent paths drawn on contour plots.
- **SVM:** hinge loss plus squared-weight regularisation, minimised with SciPy's `minimize` (not a custom solver).
- **Stack:** NumPy and Matplotlib.

![Recorded descent path](images/gradient_descent_path.png)

## Run

```sh
python3 -m venv .venv && source .venv/bin/activate
python -m pip install -r requirements.txt
jupyter notebook notebook.ipynb
```

## Limits

Seeds and package versions were not saved. The descent updates x before y rather than simultaneously. The stored SVM output reports `success: False` with a precision-loss warning, and there is no held-out accuracy. The saved images ([SVM plot](images/svm.png)) are outputs of the original run.
