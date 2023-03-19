Для запуска необходимо скачать проекты:
	server
	client1
	client2
	client3
	gateway
Необходимо, чтобы все проекты лежали в одной директории.
Далее переместить файл ./server/Docker-compose.yml в ту же директорию.
В терминале перейти в эту директорию и ввести команды:
	docker-compose build
	docker-compose up
Перейти по ссылке http://host.docker.internal:8081/
Для того, чтобы "отправить" sms, перейти по ссылке http://host.docker.internal:8082/sms
Для того, чтобы "отправить" push, перейти по ссылке http://host.docker.internal:8082/push
Для того, чтобы "отправить" email, перейти по ссылке http://host.docker.internal:8082/email
В логах будут сообщения:
	sms was sent
	push was sent
	email was sent