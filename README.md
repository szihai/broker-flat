

## Introduction

## Demo setup
The demo has 3 parts: An RSocket broker, an RSocket server that answers the query and an RSocket client with is a web server that listens to http requests and dispatches the request to the server.
![diagram](diagram.png)
All three parts are in Docker images.
Next, let's see how to deploy them.

## Simple steps

This is the simple version where most demos will be wrapped up with: Docker compose.
"By default Compose sets up a single network for your app. Each container for a service joins the default network and is both reachable by other containers on that network, and discoverable by them at a hostname identical to the container name."

* `git clone https://github.com/szihai/broker-flat.git`
* `cd broker-flat`
* `docker-compose up`   
After a while, all three containers will be up.        
Now let's test the results   
* `curl http://localhost:8181/user/2`   
Not suprisingly, you can see the result in the form of json code : 
`{"id":2,"nick":"Otha Kovacek"}`   

* Stop the containers: `docker-compose down`
## Deploy regardless of the networking

## Under the hood

## Deploy your own broker

## Try again

docker-compose up
curl http://localhost:8181/user/2




docker run  -e RSOCKET_BROKERS=tcp://47.254.15.23:9999 rsocket/rsocket-server

docker run  -e RSOCKET_BROKERS=tcp://47.254.15.23:9999 -p 8181:8181 rsocket/rsocket-client

curl http://localhost:8181/user/2


## License
Please refer to the [License](LICENSE) file.
