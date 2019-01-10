# RSocket broker bypassing network ordeal

## Overview

## Simple steps
Git clone this repo first.
## Deploy regardless of the networking

## Under the hood

## To know more

docker-compose up
curl http://localhost:8181/user/2




docker run  -e RSOCKET_BROKERS=tcp://47.254.15.23:9999 rsocket/rsocket-server

docker run  -e RSOCKET_BROKERS=tcp://47.254.15.23:9999 -p 8181:8181 rsocket/rsocket-client

curl http://localhost:8181/user/2


## License
Please refer to the [License](LICENSE) file.
