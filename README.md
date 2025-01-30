# APITempoDIO

Este repositório contém uma API de previsão do tempo desenvolvida como parte do Bootcamp Microsoft Certification Challenge #2 AZ-204 - Como Fazer o Deploy de uma API na Nuvem na Prática.

## Estrutura do Projeto

A estrutura do projeto é a seguinte:

## Descrição dos Arquivos

- **APITempoDIO/Controllers/WeatherForecastController.cs**: Controlador responsável por fornecer previsões do tempo.
- **APITempoDIO/WeatherForecast.cs**: Classe que representa a previsão do tempo.
- **APITempoDIO/Program.cs**: Arquivo principal que configura e inicia a aplicação.
- **APITempoDIO/appsettings.json** e **APITempoDIO/appsettings.Development.json**: Arquivos de configuração da aplicação.
- **APITempoDIO/Dockerfile**: Arquivo para criação da imagem Docker da aplicação.
- **pipeline.yml**: Arquivo de configuração do pipeline de CI/CD.

## Executando a Aplicação

Para executar a aplicação localmente, siga os passos abaixo:

1. Clone o repositório:
    ```sh
    git clone https://github.com/seu-usuario/APITempoDIO.git
    cd APITempoDIO
    ```

2. Restaure as dependências e compile o projeto:
    ```sh
    dotnet restore
    dotnet build
    ```

3. Execute a aplicação:
    ```sh
    dotnet run --project APITempoDIO
    ```

A aplicação estará disponível em `http://localhost:5063`.

## Endpoints

- `GET /weatherforecast`: Retorna uma lista de previsões do tempo.

## Docker

Para construir e executar a imagem Docker da aplicação, utilize os seguintes comandos:

1. Construa a imagem Docker:
    ```sh
    docker build -t apitempodio .
    ```

2. Execute o container:
    ```sh
    docker run -p 8080:80 apitempodio
    ```

A aplicação estará disponível em `http://localhost:8080`.

## Pipeline de CI/CD

O arquivo [pipeline.yml](http://_vscodecontentref_/12) configura um pipeline de CI/CD utilizando Azure Pipelines. Ele inclui etapas para restaurar, compilar, testar e publicar a aplicação Docker.

## Contribuição

Sinta-se à vontade para contribuir com este projeto. Abra uma issue ou envie um pull request com melhorias e correções.

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
