# SciSharpCube
Quickly experience all the latest features of SciSharp Machine Learning tools in docker container.

##### Get source code
```shell
git clone https://github.com/SciSharp/SciSharpCube
cd SciSharpCube
```
##### Build docker image
```shell
docker pull microsoft/dotnet
docker build -f ./dockerfiles/TensorFlow.dockfile -t scisharp-tensorflow .
```
##### Start a container
```shell
docker run --name scisharp-tensorflow -it -p 5005:5005 scisharp-tensorflow
```
##### Re-enter container
```shell
docker start scisharp-tensorflow -i
```

##### Start Jupyter Notebook
```shell
jupyter notebook --allow-root
```
