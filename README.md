# useringo.github.io
A simple frontend to interface with Ringo's API. Somewhat hacky, but it works.

### Running locally
If you want to set up the frontend to run on your local machine alongside your own copy of the Ringo build server, you're going to need to grab the ngrok localhost tunnel (highlighted in red) given by the build server. 

![build server](http://puu.sh/lCdsF/51822081e0.png)

Once you have the build server's ngrok tunnel URL, you can change the ```BALANCER_URL``` in the ```local_config.js``` file within the frontend project directory to that URL. This will tell the frontend to send all of it's requests to your local server. To run the frontend (and this is where it's super hacky), simply run the following within the frontend project directory:

```$ python -m SimpleHTTPServer```
