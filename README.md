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
docker run --name scisharp-tensorflow -it -p 8888:8888 scisharp-tensorflow
```
Now you can open the Jupyter link printed out in the console in your browser. Congratulations, 
you are running SciSharp/TensorFlow.net in Jupyter


##### Re-enter container
If you ever exit the container with Control-C you can re-enter it with the following command.

```shell
docker start scisharp-tensorflow -i
```
