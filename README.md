# NikitaApi
How to launch api:

There is a Dockerfile in the root directory.

So in the root directory:

docker build . -t [NAME_OF_IMAGE]

docker run -d --name [CONTAINER_NAME] -p 80:80 [NAME_OF_IMAGE]

then one could get pull reserves using:

curl 0.0.0.0
or
going to http://localhost:80

API provides reserves for usdc/usdt in the following format:
{"token1": int, "token2": int, "timestamp": int}
