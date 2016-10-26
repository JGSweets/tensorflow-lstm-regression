# tensorflow-lstm-regression

This is an example of a regressor based on recurrent networks:

The objective is to predict continuous values, sin and cos functions in this example, based on previous observations using the LSTM architecture. An example of using LSTM networks to make multilayer predictions (lstm-weather.ipynb) is provided in the project as well as using RNN without deep layers (lstm-sin.ipynb)

![weather predict](http://deephash.com/wp-content/uploads/2016/10/Screen-Shot-2016-10-16-at-3.22.08-PM.png "weather predict")

## Docker container

```
$ docker run -d -p 8888:8888 claytantor/tensorflow-lstm-regression:latest
```

### Version Info

* Python 2.7.11
* Pip 8.0.2
* Tensorflow 0.10 (installed from whl)
* Scipy 0.18.1
* Pandas 0.18.1
* Matplotlib 1.5.1
* Jupyter 1.0.0
* Scikit-learn 0.18
* Pysqlite 2.8.3

### Docker Hub
This project is also available as a fully configured docker container. It is possible to build it a docker container using the [Dockerfile](./Dockerfile) You can download and run it from docker hub at the project page: [claytantor/tensorflow-lstm-regression](https://hub.docker.com/r/claytantor/tensorflow-lstm-regression/)

## Building The Project 

### Create a Virtual Environment
It is reccomended that you create a virtualenv for the setup since this example is highly dependant on the versions set in the requirements file.

```
$ virtualenv ~/python/ltsm
$ source ~/python/ltsm/bin/activate
(ltsm) $
```

### Install Requirements
This example depends on **tensorflow-0.10.0rc0** to work. You will first need to install the requirements. You will need the appropriate version of tensorflow for your platform, this example is for mac. For more details goto [TAG tensorflow-0.10.0rc0 Setup](https://github.com/tensorflow/tensorflow/blob/v0.10.0rc0/tensorflow/g3doc/get_started/os_setup.md)
```
(ltsm) $ wget https://storage.googleapis.com/tensorflow/mac/cpu/tensorflow-0.10.0rc0-py2-none-any.whl
(ltsm) $ pip install -U ./tensorflow-0.10.0rc0-py2-none-any.whl
(ltsm) $ pip install -r ./requirements.tx
```

### Running on Jupyter
Three Jupyter notebooks are provided as examples on how to use lstm for predicting shapes. They will be available when you start up Jupyter in the project dir.

```
(ltsm) $ jupyter notebook
```


## Other Reading
For more details please look at this blog post [Sequence prediction using recurrent neural networks(LSTM) with TensorFlow](http://mourafiq.com/2016/05/15/predicting-sequences-using-rnn-in-tensorflow.html)
