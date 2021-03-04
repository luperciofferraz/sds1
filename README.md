# SDS1 (Games)

Sistema de um catálogo de Games e seus respectivos Gêneros, onde o usuário escolhe o Jogo de sua preferência e também pode consultar o resultado das escolhas de outros usuários.

O projeto está subdividido da seguinte forma:

- Front-Web: corresponde ao Front-End da aplicação, desenvolvido em React.
- Front-Mobile: corresponde ao projeto Mobile, desenvolvido em React Native (Ainda não disponível)
- Back-end: corresponde ao Back-End do projeto, desenvolvido em Spring Boot (Java).

Desenvolvido utilizando Spring Boot, o Back-End do projeto foi concebido utilizando as melhores práticas em arquitetura de API java, sendo dividido nas seguintes camadas:

- Resource: Classes de Endpoints, onde são recebidas as requisições dos usuários.
- DTO: Classes que montam o conteúdo e o formato das informações que serão trafegadas entre o Cliente e o Servidor, trazendo os seguintes benefícios.
  - Recebimento e envio somente da informação necessária.
  - Evitando o contato direto à camada de acesso ao Banco de Dados e seu contexto de persistência.
  - Enviando respostas ao cliente em um formato padronizado e amigável.
- Repository: Camada de Acesso aos dados, padrão Repository do Spring Boot.
- Entity: Classes de Entidades do Banco de Dados
- Service: Classes de Serviços quem fazem o 'meio-de-campo' entre as Classes Resource e Repository.
