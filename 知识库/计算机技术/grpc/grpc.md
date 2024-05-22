# grpc

python -m grpc_tools.protoc -I. --python_out=. --grpc_python_out=. ./hello.proto

python service.py

退出时用Ctrl +C