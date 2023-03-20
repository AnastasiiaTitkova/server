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
Eureka Server: http://host.docker.internal:8081/
Для того, чтобы "отправить" sms, выполните запрос POST http://host.docker.internal:8082/sms
Для того, чтобы "отправить" push, выполните запрос POST http://host.docker.internal:8082/push
Для того, чтобы "отправить" email, выполните запрос POST http://host.docker.internal:8082/email
В логах будут сообщения:
	sms was sent
	push was sent
	email was sent