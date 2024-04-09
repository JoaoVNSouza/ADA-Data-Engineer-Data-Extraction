# Projeto de Extração de Dados do curso de Engenharia de Dados na ADA
Neste projeto, estamos focados na extração de dados utilizando a NEWS API para alimentar nosso pipeline de dados. Além disso, vamos utilizar a metodologia ELT (Extract, Load, Transform) para processar e integrar os dados coletados.

### Sobre ELT
ELT é uma abordagem de integração de dados que se diferencia do ETL (Extract, Transform, Load) tradicional, principalmente na ordem das operações. Enquanto no ETL os dados são extraídos, transformados e então carregados no destino final, no ELT os dados são extraídos, carregados diretamente no destino e, em seguida, transformados dentro do próprio ambiente de armazenamento. Isso é especialmente útil quando lidamos com grandes volumes de dados e sistemas de armazenamento distribuídos.

### Objetivos do Projeto
O objetivo principal deste projeto é extrair dados da NEWS API, utilizando a chave de acesso (API_KEY) fornecida após o login. Em seguida, esses dados serão carregados em um repositório de dados central, onde serão submetidos a processos de transformação conforme necessário para atender aos requisitos analíticos e de negócios.

### Requisitos para acessar a API da NEWS API:
* É necessário fazer login e gerar uma API_KEY.
* Inserir essa API_KEY no arquivo api_key.

### Organização dos Arquivos do ELT
A organização dos arquivos do ELT seguirá um padrão que facilite o gerenciamento e manutenção do pipeline de dados baseado na arquitetura Midellion. Isso pode incluir:

* Scripts de Extração (landing_zone): Contendo código para extrair dados da API e salvar localmente no formato csv.
* Scripts de Carregamento (bronze): Responsáveis por carregar os dados extraídos em um repositório central no formato parquet.
* Scripts de Limpeza (silver): Após o carregamento, os dados podem passar por processos de limpeza no formato parquet.
* Scripts de Transformação (gold): Após os dados serem limpos, será aplicado transformações de agregações conforme necessário para atender aos requisitos analíticos também no formato parquet.


Ao seguir essa organização, garantimos que nosso pipeline de dados seja robusto, escalável e fácil de manter ao longo do tempo.

Este projeto representa um passo importante no desenvolvimento de habilidades em Engenharia de Dados e na aplicação prática de conceitos como ELT para lidar com dados do mundo real.

