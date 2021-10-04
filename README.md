# rotten-potatoes


git clone https://github.com/challengekubedev/rotten-potatoes.git

kind delete cluster --name meucluster

kind create cluster --name meucluster --config cluster.yaml

gubctl nodes

docker container ls

##criar o Docker file

docker build -t richardsonbruno/rotten-potatoes:v1 . 

docker image ls

docker login

docker push richardsonbruno/rotten-potatoes:v1

dockert tag richardsonbruno/rotten-potatoes:v1 richardson/rotten-potatoes:latest

docker push richardsonbruno/rotten-potatoes:latest

##edita deployment.yaml

kubeclt apply -f deployment.yaml

kubeclt get pods

kubeclt get all

kubeclt port-forward	svc/mongodb 27017:27017

##edita deployment.yaml

kubeclt apply -f deployment.yaml

kubeclt get all
