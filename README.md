# QP-website

В этом репозитории две ветки - stage и prod.

Ветка stage отвечает за код на staging(217.182.77.181:80) сервере. Каждый раз, когда программист делает git push origin в эту ветку автоматически запускается новый Джоб в Jenkins и деплоит код на staging server. Всегда, в конце страницы будет отображено информацию о сборке и о текущей ветке (Branch: origin/stage Build id: 21).
Так же, если билд не прошёл или нестабилен то на email программиста и девопса приходит уведомление о том, что с билдом случилось и приглашение посмотреть логи в Jenkins. Когда билд переходит в статус Success об этом тоже прийдёт оповещение на email программисту работающему в этой ветке.

Ветка prod отвечает за production(137.74.45.147:80) сервер. Здесь всё настроеноточно так же, как и в stage-ветке, только не добавляется в конце страницы информация о билде. Перед тем, как делать git merge код должен обязательно пройти ревью у девопс-инженера. 

Просьба к программисту - всегда писать commit messages.
