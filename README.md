# Settings API

Settings API is to be used behind Micro API gateway.

## Getting started

1. Install Consul

	Consul is the default registry/discovery for go-micro apps. It's however pluggable.
	[https://www.consul.io/intro/getting-started/install.html](https://www.consul.io/intro/getting-started/install.html)

2. Run Consul
	```
	$ consul agent -server -bootstrap-expect 1 -data-dir /tmp/consul
	```
3. Quick run

	```
	go run main.go
	```
4. Download and start the service

	```shell
	go get github.com/kazoup/settings-api
	message-api
	```

	OR as a docker container

	```shell
	docker run kazoup/settings-api --registry_address=YOUR_REGISTRY_ADDRESS
	```
