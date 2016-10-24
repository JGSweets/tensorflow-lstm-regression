# tensorflow-lstm-regression

This is an example of a regressor based on recurrent networks:

The objective is to predict continuous values, sin and cos functions in this example, based on previous observations using the LSTM architecture.

## Building the docker image from source

```
18:45:15 ~/data/github/claytantor/tensorflow-lstm-regression {master} $ docker build .
```

docker run -d -p 8888:8888 claytantor/tensorflow-lstm-regression:latest 
