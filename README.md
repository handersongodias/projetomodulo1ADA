
<h5>Ambiente com RabbitMq, Minio, Redis, uma aplicação de envio e outra de consumo de filas que verificam os valores das transações e validam se houve fraude, com utilização de cache e arquivos </h5>

>// Utilizar o VSCode <br>
>// no terminal executar o comando docker compose -f "Docker-compose.yaml" up -d --build <br>
>// apos os serviços serem iniciados, verificar os logs do Send e Received , la consta as transações de envio e consumo. <br>

>// A Aplicação Send termina apos enviar os dados do arquivo list.json. <br>
>// A Aplicação Received, consome os dados enviados pela Send, e caso seja identificado fraude , é gerado arquivo e enviado para o Minio. <br>

>// As aplicações só serão incializadas apos os serviços RabbitMQ , Redis e Minio estiverem iniciados e operacionais.<br>
>// Aplicação simula envio de transações de credito e avalia se há fraudes, atraves da analise dos valores enviados nas transações, o dados são carregados do arquivo list.json.<br>
