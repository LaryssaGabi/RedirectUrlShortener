# Serverless URL Shortener with AWS Lambda and S3

Este projeto utiliza **AWS Lambda** para a criação de funções serverless e **Amazon S3** para armazenamento escalável e seguro. Ao longo do desenvolvimento, você aprenderá a configurar e integrar esses serviços para construir um sistema de encurtamento de URLs eficiente e escalável.

## Funcionalidades

1. **Configuração da Conta na AWS**  
   - Criação da conta na AWS.
   - Entendimento do papel das funções serverless no desenvolvimento de sistemas escaláveis.

2. **Primeira Função Lambda: "Hello World"**  
   - Criação de uma função simples para familiarização com a plataforma AWS Lambda.

3. **Função `createShortUrlLambda`**  
   - Responsável por gerar URLs encurtadas de forma dinâmica.
   - Configuração do projeto para:
     - Receber e tratar requisições.
     - Realizar o parse dos dados.
     - Extrair informações necessárias.
     - Gerar UUIDs únicas para identificar URLs.

4. **Integração com o Amazon S3**  
   - Exploração do papel do S3 na arquitetura serverless.
   - Configuração de um bucket para armazenamento de dados das URLs encurtadas.
   - Integração da função `createShortUrlLambda` com o bucket.

5. **Testes e Validação**  
   - Execução de testes para garantir o funcionamento correto do sistema de encurtamento de URLs.

## Etapas de Desenvolvimento

1. **Criar uma Conta na AWS**  
   Configure sua conta na AWS para acessar os serviços Lambda e S3.

2. **Criar a Função `Hello World`**  
   Teste inicial para validar a configuração do ambiente Lambda.

3. **Desenvolver `createShortUrlLambda`**  
   - Receber requisições HTTP.
   - Processar dados da URL fornecida.
   - Gerar UUIDs únicas para cada URL encurtada.

4. **Configurar o Amazon S3**  
   - Criar um bucket S3 para armazenar informações de URLs.
   - Integrar a função Lambda com o bucket.

5. **Testar e Validar o Sistema**  
   Realizar testes práticos para verificar o correto funcionamento do sistema de encurtamento de URLs.

----
