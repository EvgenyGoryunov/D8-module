# D6-module-v4
логин / пароль админа
adm@adm.adm / admin

при регистрации - приветственное письмо с ссылкой подтвержения реально отправляется, в консоль не выводится
при добавлении новой статьи - письма отправляются подписчикам реально + вывод в консоль
при еженедельной рассылки - письма выводятся только в консоль, если делать реальную рассылку блокирует яндекс, говоря, что занимаетесь спамом
чтоб запустить недельную реальную рассылку нужно раскоментить код 108 строчки файла newapp\management\commands\runapscheduler.py

чтоб запустить основной сервер 
py manage.py runserver
чтоб запустить дополнительную консоль для недельной рассылки (настроена сейчас на рассылку каждые 10 секунд, для теста, а рядом есть закоменченный код для недельной рассылки)
py manage.py runapscheduler

вывод в консоль максильно много инфы, что не получать бан от яндекса за спам-рассылку, как он считает

ссылки на статьи в рассылке подписчикам действуют, если ваш сервер и порт http://127.0.0.1:8000/
