Esse projeto é só para testar o funcionamento do Airflow com Docker
Esse teste fiz no windows 11 
1) instalar o Docker desktop
2) Criar pasta em c:\airflow e dentro dela criar as pastas dags, logs, plugins, e config essa pasta sincroniza com o Docker
3) Na pasta c:\airflow colocar o arquivo docker-compose.yaml pode ser copiado aqui do meu git ou original https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html
4) Com Docker aberto no powersell ou cmd rode o comando => docker compose up airflow-init (ira baixar container), depois rode => docker compose up -d
5) Pronto agora vc deve ter os serviços rodando, coloque os dags (tenho um de exemplo aqui no git)
6) Para usar a API do exemplo Dag_wether_data, crie um a conta no site https://home.openweathermap.org/api_keys e copie a key  
7) Obs1:. caso queira rodar o airflow em uma porta que não seja a padrão 8080, editar o arquivo airflow.cfg esse arquivo fica na pasta /opt no serviço airflow-airflow-webserver-1
8) Obs2:. comando para acessar a pasta do docker exec -it airflow_docker-airflow-webserver-1 /bin/bash
