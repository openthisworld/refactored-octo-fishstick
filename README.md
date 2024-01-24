# refactored-octo-fishstick
nginx + terraform + github actions



git clone [URL вашого репозиторію]
cd [назва папки репозиторію]

docker build -t nginx-custom .

docker run -d -p 8080:80 --name nginx-container nginx-custom

У цій команді 8080:80 вказує на те, що контейнер буде доступний на порту 8080 вашого локального комп'ютера.

Відкрийте ваш веб-браузер та перейдіть за адресою http://localhost:8080. Ви повинні побачити Nginx привітальну сторінку або результат роботи вашого додатку, який проксується через Nginx.

docker stop nginx-container
docker rm nginx-container
