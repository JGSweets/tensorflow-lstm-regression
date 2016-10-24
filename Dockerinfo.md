# tensorflow-lstm-regression for Docker

This is an example of a regressor based on recurrent networks:

The objective is to predict continuous values, sin and cos functions in this example, based on previous observations using the LSTM architecture. An example of using LSTM networks to make multilayer predictions (lstm-weather.ipynb) is provided in the project as well as using RNN without deep layers (lstm-sin.ipynb)

## Running the container

```
$ docker run -d -p 8888:8888 claytantor/tensorflow-lstm-regression:latest
```

# Version Info

* Python 2.7.11
* Pip 8.0.2
* Tensorflow 0.10 (installed from whl)
* Scipy 0.18.1
* Pandas 0.18.1
* Matplotlib 1.5.1
* Jupyter 1.0.0
* Scikit-learn 0.18
* Pysqlite 2.8.3
