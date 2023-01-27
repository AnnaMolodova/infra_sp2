# Api_Yamdb
API_yautube - это API интерфейс предназначеный для развития функционала сайта.

###  Технологии в проекте: <img src="https://media.giphy.com/media/WUlplcMpOCEmTGBtBW/giphy.gif" width="30"> 
- _Django_ 🧡
- _Gunicorn_ 💚
- _NGINX_ 💜
- _POSTGRES_ 💙

###  Как запустить :
 Для начала необходимо [скачать](https://www.docker.com) Docker для своей ОС 
 
1.  Склонируйте проект к себе на компьютер

`git clone git@github.com:AnnaMolodova/infra_sp2.git`

2.  Откройте терминал и перейдите в директорию, которую скачали. Переход осуществляется с помощью команды `cd <Путь до infra_sp2>`

3. Перейдите в директорию api_yamdb
    `cd api_yamdb`
  4. Запустите сборку образа
     `docker build -t yamdb .`
5.  Переходим на директорию выше
     `cd ..`  и переходим в папку infra `cd infra`
 6. Запускаем Docker-compose командой `docker-compose up` 
 7. Выполняем миграции 
 `docker-compose exec web python manage.py migrate`
8. Создаем суперюзера 
`docker-compose exec web python manage.py createsuperuser`
9. Собираем статику
`docker-compose exec web python manage.py collectstatic --no-input`
 
  10. Зайдите на _[http://localhost/admin/](http://localhost/admin/)_ и авторизуйтесь

*Поздравляю, вы успешно вошли в систему, теперь вы можете заполнять, создавать и выкладывать различные произведения*

 ***Если вы хотите узнать, как пользоваться API для нашего приложения, то можете нажать [сюда](https://github.com/AnnaMolodova/api_yamdb)***

   *С вами был джедай Молодова Анна, `да прибудет с вами сила`*

<div align="center">  <img src="https://media.giphy.com/media/vLlpbDafjgHystuJ0a/giphy.gif" width="300" height="300"/>  </div>
