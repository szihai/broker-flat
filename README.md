# broker-flat
RSocket broker flat network implementing service mesh




docker-compose up
curl http://localhost:8181/user/2




docker run  -e RSOCKET_BROKERS=tcp://47.254.15.23:9999 rsocket/rsocket-server

docker run  -e RSOCKET_BROKERS=tcp://47.254.15.23:9999 -p 8181:8181 rsocket/rsocket-client

curl http://localhost:8181/user/2
