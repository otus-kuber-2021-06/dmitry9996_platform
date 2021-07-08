# dmitry9996_platform
dmitry9996 Platform repository

Выполнено ДЗ №2

Пункт 1:

Уcтановлен kubectl;
Установлен minikube;
создан Dockerfile, в котором будет описан образ web сервера на nginx;
создана дериктория kubernetes-intro/web;
собран докер образ и размешен в Container Registry Docker Hub https://hub.docker.com/layers/json1/web-app/0.12/images/sha256-416260247bf4f29aa89070bd5c3fdd9a7dee9c9a37f9de19df07ea1bffe90253?context=explore;
Написан манифест web-pod.yaml;

Пункт 2

Как запустить проект:
Поместить манифест web-pod.yaml в k8s;
Создать pod коммандой kubectl apply -f web-pod.yaml;
Как проверить работоспособность:
Открыть порт для pod коммандой: kubectl port-forward --address 0.0.0.0 pod/web 8000:8000
Перейти по ссылке http://localhost:8080
PR checklist:
 Выставлен label с темой домашнего задания