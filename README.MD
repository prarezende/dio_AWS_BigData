<h1 align="center">
    <img alt="LOGO" height="90px" src="https://hermes.digitalinnovation.one/site/images/logo-footer.png" />
    <br>
    
# DIO-AWS-BigData

Reposit�rio de c�digo do Dio Live Coding com AWS EMR e Python
. Curso ministrado por Cassiano Brexbit. 
Neste reposit�rio h� os arquivos de configura��o e execu��o de an�lise de dados.


## Instru��es

* Acessar S3: https://s3.console.aws.amazon.com/s3/ 
  * Criar estrutura de data lake : _dio-live-datalake_
  * Criar estrutura de pastas:
    * _data_
    * _output_
    * _temp_
* Acessar EMR: https://console.aws.amazon.com/elasticmapreduce/
    * O cluster ser� criado pelo MrJob e n�o pelo console
    * Infraestrutura como c�digo 
* Criar chave SSH
    * Acessar  Console do EC2: https://console.aws.amazon.com/ec2/ -> Key Pairs -> Create Key Pair	
    * Download .pem file
* Obter Id e chave secreta AWS para configurar MrJob
   * Profile
   * My Security Credentials: https://console.aws.amazon.com/iam/home?region={region}#/security_credentials
   * Access Keys - Create new access key
   * Fazer download - �nica chance de visualizar
* Ambiente linux
   * Criar ambiente virtual python: _virtualenv --python=python3.6 venv_diolive_
   * Acessar com o vs code
* Instalar vscode no Ubuntu
   *  code .
* Criar algoritmo de an�lise de palavras
   * dio-live-wordcount-test.py
   * map-reduce-count : contar
   * Instalar boto3: _pip install boto3_
   * Instalar mrjob: _pip install mrjob_
* Acessar S3
   * Upload de arquivo para o bucket
* Ambiente virtual python: source venv_teste/bin/activate
  * _nano ~/.mrjob.conf_
  * _python3 dio-live-wordcount-test.py -r emr s3://{your_s3_bucket_name}/data/SherlockHolmes.txt --output-dir=s3://{your_s3_bucket_name}/output/logs1 --cloud-tmp-dir=s3://{your_s3_bucket_name}/temp/_




## Autora

| [<sub>Patricia Albuquerque</sub>](https://github.com/prarezende) |
| :---: |
|[Linkedin](https://www.linkedin.com/in/patricia-albuquerque-ti-30250)|
