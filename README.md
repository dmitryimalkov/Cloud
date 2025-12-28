# Cloud
Test cloud solutions with Giga AI
.ssh : ssh-pk-15765d name id_ed25519.pub
Разверните ресурсы в облаке
Задача: создадать бесплатную виртуальную машину, назначить ей публичный IP-адрес и настроить правила фильтрации трафика через него.
Имя хоста: wordpress-server
Имя пользователя: login : user1
Пароль : Volga430m!
Зона доступности: ru.AZ-2
Публичный адрес: 45.151.30.147
Группа безопасности: wordpress-server
Пробный вход был в 18:10- 23 декабря. Виртуальная машина остановлена

mysql login wp_user
mysql pass Volga430m!

Настройте WordPress с помощью шаблона wp-config-sample.php. Выполните команды копирования и заполнения шаблонного файла. В <password> укажите пароль для пользователя wp_user, заданный при настройке базы данных.
sudo sed -i -e "s/password_here/Volga430m!/g" /var/www/html/wp-config.php

Настройка доменного имени
45.151.30.147.nip.io

Не удалось запустить wordpress:
Requesting a certificate for 45.151.30.147.nip.io
An unexpected error occurred:
There were too many requests of a given type :: too many certificates (25000) already issued for "nip.io" in the last 168h0m0s, retry after 2025-12-28 09:18:47 UTC: see https://letsencrypt.org/docs/rate-limits/#new-certificates-per-registered-domain
