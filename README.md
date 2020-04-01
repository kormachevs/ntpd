# ntpd
Роль просмотрел, странностей не нашел.

Установка роли:

    git clone https://github.com/kormachevs/ntpd.git

    cd ./ntpd

#### Поправить hosts, заполнить своими данными

    ansible-playbook play_ntpd.yaml

### Переменные, которые можно передать как EXTRA_VARS, или поправить в playbook-е.

    ntp_timezone: Europe/Moscow
    ntp_pools:
      - 0.ru.pool.ntp.org
      - 1.ru.pool.ntp.org

Тестирование роли на OS: Ubuntu 16.04, Ubuntu 18.04
