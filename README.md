# rotten-potatoes


git clone https://github.com/challengekubedev/rotten-potatoes.git

kind delete cluster --name meucluster

kind create cluster --name meucluster --config cluster.yaml

kubeclt nodes

docker container ls

## criar o Docker file

```
FROM python: 3.8
WORKDIR /app-web
COPY requirements.txt .
RUN python -m pip install -r requirments
COPY . .
EXPOSE 5000
CMD ["gunicorn", "--workers=3", "--bind", "0.0.0.0:5000", "app:app"]
```

docker build -t richardsonbruno/rotten-potatoes:v1 . 

docker image ls

docker login

docker push richardsonbruno/rotten-potatoes:v1

dockert tag richardsonbruno/rotten-potatoes:v1 richardson/rotten-potatoes:latest

docker push richardsonbruno/rotten-potatoes:latest

## edita deployment.yaml

kubeclt apply -f deployment.yaml

kubeclt get pods

kubeclt get all

kubeclt port-forward	svc/mongodb 27017:27017

## edita deployment.yaml

kubeclt apply -f deployment.yaml

kubeclt get all
