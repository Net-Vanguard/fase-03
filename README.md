<details>
<summary>English version 🇺🇸</summary>

<h1 align="center">
  



  <img src="https://github.com/user-attachments/assets/54f21caa-4fdb-4cb8-a282-104bda580d30" alt="FCG Logo" width="180">
  



  FIAP Cloud Games (FCG) - Phase 3
  



</h1>

<h4 align="center">
Service developed as part of the Phase 3 Tech Challenge — <a href="https://www.fiap.com.br/" target="_blank">FIAP</a> Postgraduate in .NET Software Architecture.
</h4>



<hr>

<h2>✨ Key Features</h2>

<ul>
<li><strong>Microservices Architecture</strong>: The monolithic application was migrated to a distributed architecture with dedicated services for Users, Games, and Payments, increasing modularity and resilience.</li>
<li><strong>Advanced Search with Elasticsearch</strong>: Implementation of Elasticsearch to index game data, enabling efficient and complex queries for recommendations and metrics.</li>
<li><strong>Serverless Scalability</strong>: Use of serverless functions (e.g., AWS Lambda) for asynchronous processes like notifications and payment processing, optimizing costs and scalability.</li>
<li><strong>API Gateway</strong>: A single, secure entry point to manage and route requests to the different microservices.</li>
<li><strong>Event-Driven Architecture</strong>: Adoption of Event Sourcing to record all system state changes, ensuring auditability and data consistency.</li>
<li><strong>Enhanced Observability</strong>: Implementation of distributed logging and tracing to monitor and debug the application in a distributed environment.</li>
</ul>

<h2>🏗️ Architecture</h2>

<h3>Architectural Design</h3>

<p >
https://miro.com/welcomeonboard/WXFNR1F3MExCYnZ2RXNncGM2c1VqNHBTS29oOGlCZkkvYmk3enBzS1Y2MHl2UXh0SHMrNENtYUVodE1JZHltaXZiRXQvV3pKNm4vd3BoNG5JUXJFeHFFcHNVL25KWlpLMVp2UERoR3c1MW4xOFRFcFBPU3IxZ3NjMCtnWnYxVGZzVXVvMm53MW9OWFg5bkJoVXZxdFhRPT0hdjE=?share_link_id=35637098032
</p>

<h3>Microservices Communication Flow</h3>

<p >
[<em>(Insert your communication flow or sequence diagram here)</em>](https://miro.com/welcomeonboard/WXFNR1F3MExCYnZ2RXNncGM2c1VqNHBTS29oOGlCZkkvYmk3enBzS1Y2MHl2UXh0SHMrNENtYUVodE1JZHltaXZiRXQvV3pKNm4vd3BoNG5JUXJFeHFFcHNVL25KWlpLMVp2UERoR3c1MW4xOFRFcFBPU3IxZ3NjMCtnWnYxVGZzVXVvMm53MW9OWFg5bkJoVXZxdFhRPT0hdjE=?share_link_id=35637098032)

<code></code>
</p>

<h2>🧠 Technical Requirements</h2>

<ul>
<li><strong>Microservices</strong>:
    <ul>
    <li>Creation of at least three microservices in separate repositories (e.g., Users, Games, Payments).</li>
    </ul>
</li>
<li><strong>Elasticsearch</strong>:
    <ul>
    <li>Indexing of game data for efficient searching.</li>
    <li>Development of advanced queries for recommendations based on user history.</li>
    <li>Use of aggregations to generate metrics, such as most popular games.</li>
    </ul>
</li>
<li><strong>Serverless</strong>:
    <ul>
    <li>Creation of Serverless Functions (AWS Lambda or Azure Functions) for asynchronous operations.</li>
    <li>Configuration of triggers to automatically invoke functions based on events.</li>
    <li>Implementation of an API Gateway to manage and protect microservices.</li>
<li>(Optional) Configuration of JWT authentication and rate limiting.</li>
    </ul>
</li>
<li><strong>Architecture</strong>:
    <ul>
    <li>Implementation of event sourcing to log all system state changes.</li>
    <li>Improved observability with distributed logs and traces.</li>
    </ul>
</li>
</ul>

<h2>🚀 How to Use</h2>

<p><em>(Note: Since the architecture is distributed, each microservice has its own setup process. Check the README of each repository for specific details.)</em></p>

<ol>
<li><strong>Clone the repositories</strong>:
    <pre><code>Clone the User microservice repository
git clone [Link to User Microservice Repository]
   

Clone the Game microservice repository
git clone [Link to Game Microservice Repository]

Clone the Payment microservice repository
git clone [Link to Payment Microservice Repository]
    </code></pre>

</li>
<li><strong>Configure Environment Variables</strong>: Each microservice requires its own <code>.env</code> file. Refer to the <code>.env.example</code> in each repository to configure database connections, API keys, and other necessary settings.</li>
<li><strong>Run Infrastructure</strong>: Use <code>docker-compose up -d</code> in a shared infrastructure directory (if applicable) to start databases, Elasticsearch, and other services.</li>
<li><strong>Run Microservices</strong>: Navigate into each microservice's directory and run the start command (e.g., <code>npm start</code>, <code>dotnet run</code>).</li>
<li><strong>Access the Application</strong>: The services will be exposed through the API Gateway. Use the Gateway's URL to interact with the application.</li>
<li><strong>CI/CD Pipelines</strong>: CI pipelines run on pull requests, and CD pipelines deploy changes to the cloud upon merging to the main branch. Check the pipeline files (e.g., <code>.github/workflows/deploy.yml</code>) in each repository.</li>
</ol>

</details>

<h1 align="center">
  



  <img src="https://github.com/user-attachments/assets/54f21caa-4fdb-4cb8-a282-104bda580d30" alt="FCG Logo" width="180">
  



  FIAP Cloud Games (FCG) - Fase 3
  





<p align="center">
  <a href="#-principais-características">✨ Principais Características</a> •
<a href="#-arquitetura">🏗️ Arquitetura</a> •
  <a href="#-requisitos-técnicos">🧠 Requisitos Técnicos</a> •
  <a href="#-como-usar">🚀 Como Usar</a>
</p>

<hr>

<h2>✨ Principais Características</h2>

<ul>
<li><strong>Arquitetura de Microsserviços</strong>: Migração da aplicação monolítica para uma arquitetura distribuída com serviços dedicados para Usuários, Jogos e Pagamentos, aumentando a modularidade e a resiliência.</li>
<li><strong>Busca Avançada com Elasticsearch</strong>: Implementação do Elasticsearch para indexar os dados dos jogos, permitindo buscas eficientes e consultas complexas para recomendações e métricas.</li>
<li><strong>Escalabilidade com Serverless</strong>: Uso de funções serverless (ex: AWS Lambda) para processos assíncronos, como envio de notificações e processamento de pagamentos, otimizando custos e escalabilidade.</li>
<li><strong>API Gateway</strong>: Ponto de entrada único e seguro para gerenciar e rotear as requisições para os diferentes microsserviços.</li>
<li><strong>Arquitetura Orientada a Eventos</strong>: Adoção do padrão <em>Event Sourcing</em> para registrar todas as mudanças de estado do sistema, garantindo auditoria e consistência dos dados.</li>
<li><strong>Observabilidade Aprimorada</strong>: Implementação de logs e rastreamento distribuído (<em>traces</em>) para monitorar e depurar a aplicação em um ambiente distribuído.</li>
</ul>

<h2>🏗️ Arquitetura</h2>

A nova arquitetura da FCG foi desenhada para ser resiliente, escalável e observável, adotando uma abordagem baseada em eventos e microsserviços.

<h3>Diagrama da Arquitetura e Fluxo de Comunicação dos Microsserviços</h3>
<p >
https://miro.com/welcomeonboard/WXFNR1F3MExCYnZ2RXNncGM2c1VqNHBTS29oOGlCZkkvYmk3enBzS1Y2MHl2UXh0SHMrNENtYUVodE1JZHltaXZiRXQvV3pKNm4vd3BoNG5JUXJFeHFFcHNVL25KWlpLMVp2UERoR3c1MW4xOFRFcFBPU3IxZ3NjMCtnWnYxVGZzVXVvMm53MW9OWFg5bkJoVXZxdFhRPT0hdjE=?share_link_id=35637098032
<b></b>
</p>

<p><strong>Descrição do Fluxo:</strong> O cliente interage com o sistema através de um <strong>API Gateway</strong>, que roteia as requisições para os microsserviços de <strong>Usuários</strong>, <strong>Jogos</strong> e <strong>Pagamentos</strong>. O serviço de Jogos utiliza <strong>Elasticsearch</strong> para buscas, enquanto processos assíncronos são delegados a <strong>Funções Serverless</strong>. Todas as alterações de estado são registradas como eventos (<strong>Event Sourcing</strong>), e a <strong>observabilidade</strong> é garantida com logs e traces distribuídos.</p>

<p><strong>Exemplo de Fluxo (Compra de um Jogo):</strong> O usuário autenticado solicita a compra via API Gateway. O serviço de <strong>Jogos</strong> inicia a transação e publica um evento. O serviço de <strong>Pagamentos</strong> processa o pagamento e publica um evento de sucesso. Por fim, o serviço de <strong>Jogos</strong> finaliza a compra, e uma <strong>Função Serverless</strong> envia a notificação de confirmação.</p>


<h2>🧠 Requisitos Técnicos</h2>

<ul>
<li><strong>Microsserviços</strong>:
    <ul>
    <li>Criação de três microsserviços em repositórios separados (ex: Usuários, Jogos, Pagamentos).</li>
    </ul>
</li>
<li><strong>Elasticsearch</strong>:
    <ul>
    <li>Indexação de dados dos jogos para busca eficiente.</li>
    <li>Criação de consultas avançadas para recomendações baseadas no histórico do usuário.</li>
    <li>Uso de agregações para gerar métricas, como os jogos mais populares.</li>
    </ul>
</li>
<li><strong>Serverless</strong>:
    <ul>
    <li>Criação de Funções Serverless (AWS Lambda ou Azure Functions) para operações assíncronas.</li>
    <li>Configuração de gatilhos (triggers) para acionar as funções automaticamente com base em eventos.</li>
    <li>Implementação de um API Gateway para gerenciar e proteger os microsserviços.</li>
<li>(Opcional) Configuração de autenticação JWT e controle de requisições (rate limiting).</li>
    </ul>
</li>
<li><strong>Arquitetura</strong>:
    <ul>
    <li>Implementação de <em>event sourcing</em> para registrar todas as mudanças de estado do sistema.</li>
    <li>Melhora da observabilidade com logs e rastreamento distribuído (Traces).</li>
    </ul>
</li>
</ul>

<h2>🚀 Como Usar</h2>

<p><em>(Nota: Como a arquitetura é distribuída, cada microsserviço possui seu próprio processo de setup. Verifique o README de cada repositório para detalhes específicos.)</em></p>

<ol>
<li><strong>Clone os repositórios</strong>:
    <pre><code>Clone o repositório do microsserviço de Usuários
git clone [[Link para o repositório do Microsserviço de Usuários](https://github.com/Net-Vanguard/Fiap-Users.git)]
   

Clone o repositório do microsserviço de Jogos
git clone [[Link para o repositório do Microsserviço de Jogos](https://github.com/Net-Vanguard/Fiap-Games.git)]

Clone o repositório do microsserviço de Pagamentos
git clone [[Link para o repositório do Microsserviço de Pagamentos](https://github.com/Net-Vanguard/Fiap-Payments.git)]
    </code></pre>

</li>
<li><strong>Configure as Variáveis de Ambiente</strong>: Cada microsserviço exige um arquivo <code>.env</code> próprio. Consulte o <code>.env.example</code> em cada repositório para configurar as conexões de banco de dados, chaves de API e outras definições.</li>
<li><strong>Execute a Infraestrutura</strong>: Utilize <code>docker-compose up -d</code> em um diretório de infraestrutura comum (se aplicável) para iniciar os bancos de dados, Elasticsearch, etc.</li>
<li><strong>Execute os Microsserviços</strong>: Navegue até o diretório de cada microsserviço e execute o comando de inicialização (ex: <code>npm start</code>, <code>dotnet run</code>).</li>
<li><strong>Acesse a Aplicação</strong>: Os serviços serão expostos através do API Gateway. Utilize a URL do Gateway para interagir com a aplicação.</li>
<li><strong>Pipelines de CI/CD</strong>: As pipelines de CI são executadas em pull requests e as de CD realizam o deploy na nuvem após o merge na branch principal. Consulte os arquivos de pipeline (ex: <code>.github/workflows/deploy.yml</code>) em cada repositório.</li>
</ol>
