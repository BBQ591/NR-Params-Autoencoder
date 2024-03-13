2 Layer Individual Generator: Used to generate data for 2 layer systems
3 Layer Individual Generator: Used to generate data for 3 layer systems
Big Generator: Used to generate a big, uncondensed dataset, covering as much data as possible
AEMLPPoly: Normal Autoencoder + MLP
VAEMLPPoly: Variational Autoencoder + MLP

Instructions to generate results: First, create the dataset using the Big Generator code. Train an AE+MLP on this training data and then generate the predicted results of an experimental NR curve. This set of parameters from the MLP should be relatively close to the truth values, but not super close. To increase the accuracy, put the predicted values into an Individual Generator (depending on how many layers are in the experimental film) and generate a smaller dataset. Continue this process until the predictions are very accurate.