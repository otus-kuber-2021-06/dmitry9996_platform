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

 PR checklist:
      Выставлен label с темой домашнего задания
