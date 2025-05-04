# Задание 2

## Запуск кластера

 minikube start --vm-driver=virtualbox --addons=metrics-server --no-vtx-check --memory=8192 --cpus=4


## Запуск сервиса

 kubectl apply -f deployment.yaml

 kubectl apply -f service.yaml
 
 minikube service scaletestapp --url
 
## Настройки масштабирования 

 minikube addons enable metrics-server
 
 kubectl apply -f hpa.yaml
 
## Результаты

До нагрузки:



Во время нагрузки:


