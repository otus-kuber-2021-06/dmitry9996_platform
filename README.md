Выполнено ДЗ №3

task01:

- Создан sa bob с CluterRole admin

- Создан sa dave без (cluster)rolebinding

task02:

- Создан namespace prometheus

- Создан sa carol

- Создана кластерная роль sa-role с правами выполнять get, list, watch над ресурсом pod

- Создан ClusterRoleBinding, назначающий кластерную роль sa-role группе сервисных аккаунтов в namespace prometheus

task03:

- Создан namespace dev

- Создан sa jane

- Создан ClusterRoleBinding, назначающий кластерную роль admin sa jane

- Создан sa ken

- Создан ClusterRoleBinding, назначающий кластерную роль view sa ken

<<<<<<< HEAD
- Открыть порт для pod коммандой: kubectl port-forward --address 0.0.0.0 pod/web 8000:8000Перейти по ссылке http://localhost:8080


PR checklist:
 Выставлен label с темой домашнего задания


Выполнено ДЗ №4

task01:

- Создан sa bob с CluterRole admin

- Создан sa dave без (cluster)rolebinding

task02:

- Создан namespace prometheus

- Создан sa carol

- Создана кластерная роль sa-role с правами выполнять get, list, watch над ресурсом pod

Создан ClusterRoleBinding, назначающий кластерную роль sa-role группе сервисных аккаунтов в namespace prometheus

task03:

- Создан namespace dev

- Создан sa jane

- Создан ClusterRoleBinding, назначающий кластерную роль admin sa jane

- Создан sa ken

- Создан ClusterRoleBinding, назначающий кластерную роль view sa ken

PR checklist: Выставлен label с темой домашнего задания





Выполнено ДЗ №5


- Создали манифест deployment с указанием стратегии обновления

- Создали манифест сервиса с ClusterIP web-svc-cip

- Переключили kube-proxy в режим `ipvs`
 
- Очистили правила iptables в minikube

- Установили и настроили работу ingress-nginx


Выполнено ДЗ №6

- Развернули MINIO используя StatefullSet



Выполнено ДЗ №8

- Создан CRD для MySQL:
- Добавлена проверка наличия всех необходимых строчек в спецификации;
- Создали custom controller на python;
- Создали docker образ json1/mysql-operator:v0.0.1 оператора mysql;
- Проверили работу оператора.



### Как запустить: 
- Запустить minikube
- Установить python модули:
  - kopf (https://kopf.readthedocs.io/en/latest/install/)
  - kubernetes
  - jinja2
  - pyyaml

#### Ручной запуск (проверка работы оператора)
- В отдельной консоли запустить наш контроллер: `kopf run mysql-operator.py`
- В другом окне консоли применить манифест cr: `kubectl apply -f deploy/cr.yml`

=======
 PR checklist:
      Выставлен label с темой домашнего задания
>>>>>>> 8fe819c6762b09aceaa330c6df5102534550d97a
