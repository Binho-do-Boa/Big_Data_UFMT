Esse projeto é só para testar o funcionamento do Airflow com Docker
Esse teste fiz no windows 11 
1) instalar o Docker desktop
2) Criar pasta em c: airflow e dentro dela ciars as pastas dags, logs, plugins, e config essa pasta crincroniza com o Docker
3) Na pasta c:\airflow colocar o arquivo docker-compose.yaml pode ser copiado aqui do meu git ou original https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html
4) Com Docker aberto no powersell ou cmd rode o comando => docker compose up airflow-init (ira baixar container), depois rode => docker compose up -d
5) Pronto agora vc deve ter os serviços rodando, coloque os dags (tenho um de exemplo aqui no git)
6) Obs:. caso queira rodar o airflow em um porta que não seja a padrão 8080, editar o arquivo airflow.cfg esse arqui fica na pasta /opt no serviço airflow-airflow-webserver-1
