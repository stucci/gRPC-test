[Quick start | Python | gRPC](https://grpc.io/docs/languages/python/quickstart/)

setup on wsl
```shell
sudo apt install python3 python3-pip -y
pip3 install grpcio
pip3 install grpcio-tools
```

generate gRPC code
```shell
python3 -m grpc_tools.protoc -I. --python_out=. --grpc_python_out=. ./helloworld.proto
```

run gRPC application
```shell
python3 greeter_server.py
python3 greeter_client.py
```
