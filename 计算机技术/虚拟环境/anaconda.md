# anaconda

激活虚拟环境

创建虚拟环境后，我们需要激活它。在Anaconda中，可以使用以下命令来激活虚拟环境：

conda activate env_name

其中，env_name为虚拟环境的名称。执行完后，Anaconda会自动激活该虚拟环境，并且命令行的前缀会变成(env_name)。

关闭虚拟环境

在使用完虚拟环境后，我们需要关闭它。在Anaconda中，可以使用以下命令来关闭虚拟环境：

conda deactivate

执行完后，Anaconda会自动关闭当前虚拟环境。

删除虚拟环境

如果我们不再需要某个虚拟环境，可以使用以下命令来删除它：

conda remove --name env_name --all

其中，env_name为虚拟环境的名称。执行完后，Anaconda会自动删除该虚拟环境和其中的所有库。


python -m grpc_tools.protoc -I. --python_out=. --grpc_python_out=. ./hello.proto

python service.py

退出时用Ctrl +C