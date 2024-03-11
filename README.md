# DAG de Turbina Eólica

Este projeto consiste em um fluxo de trabalho (DAG) no Apache Airflow para lidar com dados de turbinas eólicas. Ele inclui tarefas para verificar a temperatura, armazenar dados em um banco de dados PostgreSQL e enviar alertas por e-mail conforme necessário.

## Pré-requisitos

Antes de executar este DAG, certifique-se de ter o Apache Airflow configurado e em execução, além de acesso a um banco de dados PostgreSQL. Certifique-se também de ter configurado as variáveis relevantes no Airflow, como o caminho do arquivo de dados e as credenciais do e-mail.

## Instalação

1. Clone este repositório:

    ```bash
    git clone https://github.com/Jezandre/windturbine.git
    ```

2. Instale as dependências necessárias do Apache Airflow.

3. Configure as variáveis relevantes no Airflow, como o caminho do arquivo de dados e as credenciais do e-mail.

4. Inicie o Airflow e adicione o DAG fornecido.

## Configuração

Antes de executar o DAG, certifique-se de configurar corretamente as variáveis no Airflow:

- `path_file`: Caminho para o arquivo de dados da turbina eólica.
- Credenciais de e-mail para envio de alertas.

## Uso

1. Inicie o DAG no painel do Apache Airflow.
2. O DAG realizará as seguintes tarefas:
   - Verificará se o arquivo de dados da turbina eólica está presente.
   - Processará o arquivo de dados.
   - Criará uma tabela no banco de dados PostgreSQL, se não existir.
   - Inserir os dados processados na tabela do banco de dados.
   - Verificará a temperatura e enviará alertas por e-mail conforme necessário.
3. Monitore a execução do DAG no painel do Apache Airflow.

## Contribuição

Contribuições são bem-vindas! Para contribuir com este projeto, siga estas etapas:

1. Faça um fork do projeto.
2. Crie uma branch para a sua feature (`git checkout -b feature/NomeDaFeature`).
3. Faça commit das suas mudanças (`git commit -am 'Adiciona nova feature'`).
4. Faça push para a branch (`git push origin feature/NomeDaFeature`).
5. Abra um pull request.

