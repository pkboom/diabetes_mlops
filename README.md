https://towardsdatascience.com/simple-model-retraining-automation-via-github-actions-b0f61d5c869c

```sh
docker build -t ppotpo/diabetes_mlops -f Dockerfile .

docker login -u ppotpo

docker push ppotpo/diabetes_mlops:latest
```

```sh
docker pull ppotpo/diabetes_mlops:latest

docker run -d -p 8000:8000 ppotpo/diabetes_mlops:latest
```

Next
Model Retraining with GitHub Actions
