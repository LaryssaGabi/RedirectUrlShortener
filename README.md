# Serverless URL Shortener with AWS Lambda, S3, and API Gateway

Este projeto utiliza **AWS Lambda**, **Amazon S3** e **API Gateway** para construir um sistema de encurtamento de URLs escalável, seguro e eficiente. Ele inclui funcionalidades para criar, armazenar e redirecionar URLs encurtadas, além de gerenciar requisições centralizadas.

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

5. **Função `redirectUrlLambda`** - **Nova Funcionalidade! Seria desse projeto** 🆕  
   - Implementação da lógica para redirecionar o usuário para a URL original a partir da URL encurtada.  
   - **Validação da Data de Expiração:** Apenas URLs válidas são redirecionadas, garantindo maior controle e segurança no sistema.

6. **Configuração do API Gateway**  
   - Centralização e gerenciamento de todas as requisições do sistema.  
   - Criação de uma estrutura robusta e segura para o serviço de encurtamento de links.

7. **Testes e Validação**  
   - Execução de testes para garantir o funcionamento correto do sistema de encurtamento e redirecionamento de URLs.

## Etapas de Desenvolvimento

1. **Criar uma Conta na AWS**  
   Configure sua conta na AWS para acessar os serviços Lambda, S3 e API Gateway.

2. **Criar a Função `Hello World`**  
   Teste inicial para validar a configuração do ambiente Lambda.

3. **Desenvolver `createShortUrlLambda`**  
   - Receber requisições HTTP.  
   - Processar dados da URL fornecida.  
   - Gerar UUIDs únicas para cada URL encurtada.

4. **Configurar o Amazon S3**  
   - Criar um bucket S3 para armazenar informações de URLs.  
   - Integrar a função Lambda com o bucket.

5. **Desenvolver `redirectUrlLambda`**  
   - Implementar a lógica de redirecionamento para a URL original.  
   - **Validar a expiração das URLs**, garantindo que apenas URLs dentro do prazo sejam redirecionadas.

6. **Configurar o API Gateway**  
   - Criar um API Gateway para gerenciar e centralizar todas as requisições do sistema.  
   - Integrar o Gateway com as funções Lambda do projeto.

7. **Testar e Validar o Sistema**  
   Realizar testes práticos para verificar o correto funcionamento do sistema de encurtamento e redirecionamento de URLs.

---

Com a adição da **função `redirectUrlLambda`**, o sistema agora é capaz de redirecionar os usuários de forma eficiente e segura, validando a data de expiração das URLs. Essa funcionalidade, combinada com
