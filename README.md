# Deullam Justi

**Desenvolvedor fullstack.** Backend em **C# / .NET** (ASP.NET Core, EF Core, Clean Architecture) e
**Node / NestJS**; frontend em **React com TypeScript**. Trabalho com PostgreSQL, SQL Server e MongoDB,
mensageria com Kafka e RabbitMQ, Docker e testes automatizados de ponta a ponta.

![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache%20Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

---

## Projetos em destaque

Os repositórios abaixo são desafios técnicos e projetos de estudo. Todos rodam em clone limpo,
com README que explica o que fazem, como subir e o que ficou de fora.

### [Deullam-Credit-Inquiry-Challenge](https://github.com/Deullam/Deullam-Credit-Inquiry-Challenge) · C# / .NET 8

API REST de créditos tributários em Clean Architecture. O `POST` responde **202 Accepted** e publica
no Kafka; um `BackgroundService` consome e grava no PostgreSQL via EF Core. Docker Compose, health
checks de liveness e readiness, e uma suíte E2E que exercita a pilha real, com broker e consumidor
de verdade, em vez de dublês.

### [Deullam.Challenge.Rigatti](https://github.com/Deullam/Deullam.Challenge.Rigatti) · NestJS + React

SaaS multi-tenant onde cada empresa gerencia seu catálogo e conversa com um agente de IA. O
isolamento entre empresas não depende de o desenvolvedor lembrar de filtrar: o `companyId` sai do
token, vai para o `AsyncLocalStorage` e o repositório base o injeta em toda consulta. O agente usa
*tool calling* para consultar o catálogo real e responde por streaming. Testes cobrem inclusive
tentativa de vazamento entre empresas por *prompt injection* e JWT forjado, adulterado e expirado.

### [Sistema-de-Enquete](https://github.com/Deullam/Sistema-de-Enquete) · PHP 8

Enquetes com MVC escrito à mão: roteador próprio, autoloader por namespace e PDO com prepared
statements. Sem framework e sem dependências de terceiros — serve para mostrar o que um framework
faz por baixo. Suíte E2E roda contra PHP e MySQL em contêiner.

---

## Como eu trabalho

- **Testes que exercitam a coisa real.** Banco, broker e servidor de verdade em contêiner, não mock
  de tudo; e testes negativos para o que precisa falhar: token forjado, isolamento entre tenants,
  entrada inválida.
- **README honesto.** Cada repositório diz o que não faz e quais são suas limitações conhecidas.
  Prefiro registrar uma dívida a escondê-la.
- **Arquitetura proporcional ao problema.** Clean Architecture onde paga o custo, e simplicidade
  onde não paga.

---

**Fullstack developer** — C#/.NET and NestJS on the backend, React with TypeScript on the frontend.

📍 Brasil · [LinkedIn](https://www.linkedin.com/in/deullam-justi)
