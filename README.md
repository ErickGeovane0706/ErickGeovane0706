<div align="center">

# Erick Geovane

### Desenvolvedor Backend Java

<p>
  <img src="https://img.shields.io/badge/Java-21-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java 21">
  <img src="https://img.shields.io/badge/Spring_Boot-3-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" alt="Spring Boot 3">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker">
</p>

<p>
  <a href="https://linkedin.com/in/erick-geovane">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="mailto:erickgeovane2002@gmail.com">
    <img src="https://img.shields.io/badge/E--mail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="E-mail">
  </a>
  <img src="https://img.shields.io/badge/Monteiro,_PB-Dispon%C3%ADvel_para_remoto-2EA44F?style=for-the-badge" alt="Disponível para trabalho remoto">
</p>

</div>

---

> Trabalho no controle financeiro de uma rede de lojas e, a partir dessa rotina, desenvolvi o
> sistema de contas a pagar que a empresa usa hoje.
>
> É de onde vem a minha forma de programar: **conheci o problema antes de escrever a solução.**

<br>

## Projetos

### 💳 [Dia de Pagar](https://www.diadepagar.com.br) — SaaS multi-tenant de contas a pagar

<sub>`produto próprio` · `no ar e em uso por uma rede de lojas` · `código privado`</sub>

Uma rede com várias lojas controlava boletos, PIX e cheques em planilha. Vencimento passava
batido, e ninguém sabia o total a pagar da semana sem somar à mão.

- **Multi-tenant com isolamento por empresa** — o `empresaId` vem do JWT e é conferido em cada
  operação. Nenhuma consulta confia em ID enviado pelo cliente.
- **Integração de pagamentos** com o gateway Asaas: checkout de assinatura, processamento de
  webhook e máquina de estados do ciclo de cobrança.
- **Agente de WhatsApp** — o usuário pergunta quanto tem a pagar na semana, por texto ou áudio,
  e recebe a resposta sem abrir o sistema. Validação de assinatura HMAC, idempotência,
  classificação de intenção e transcrição de voz.
- **Leitor de código de barras** por câmera, imagem (OCR) ou PDF, reconhecendo boleto bancário,
  convênio, DARF, GPS, DAS e GNRE.
- **327 métodos de teste em 40 classes** cobrindo isolamento multi-tenant, autenticação, upload
  e o agente de WhatsApp.

`Java 21` `Spring Boot 3` `Spring Security` `PostgreSQL` `Flyway` `React + TypeScript` `Docker`

<br>

### 🕸️ [Detector de Fraudes Financeiras](https://github.com/ErickGeovane0706/detector-fraudes-grafos) — detecção com banco de grafos

Descobrir quantos usuários compartilham o mesmo aparelho **e** enviam dinheiro para a mesma
conta exige múltiplos JOINs sobre tabelas grandes em SQL.

- **A modelagem relacional era a ferramenta errada.** Em Cypher, a mesma pergunta é uma
  travessia curta — e o custo cresce com o tamanho do padrão procurado, não com o da base.
- Identifica contas compartilhadas, dispositivos em comum e ciclos de transferência.

`Java 21` `Spring Boot 3` `FalkorDB` `Cypher` `Vaadin` `Docker`

<br>

### 🍔 [Hamburgueria](https://github.com/ErickGeovane0706/Hamburgueria) — gestão e PDV

Saber quanto comprar de cada ingrediente depende de quanto se pretende produzir — e ninguém
faz essa conta à mão todo dia.

- **Previsão de produção** — a partir da quantidade planejada, o sistema explode a ficha
  técnica, soma a necessidade por ingrediente e aponta falta e sobra antes da compra.
- Ponto de venda, fechamento de caixa e relatórios com ticket médio e distribuição por forma
  de pagamento.
- Empacotável como aplicativo desktop via Tauri, porque o balcão da loja não depende de
  navegador aberto.
- **62 métodos de teste automatizados.**

`Java 21` `Spring Boot 3` `React 18` `PostgreSQL` `Tauri`

<br>

### 💇 [Syra Estética](https://github.com/ErickGeovane0706/syra) — agendamento e loja

Sistema de agendamento de serviços e catálogo de produtos para um salão de estética,
publicado em cloud.

- Login com Google OAuth2 e sessão via JWT, com agenda de horários configuráveis e painel
  administrativo.
- Deploy distribuído: Vercel no frontend, Render no backend e Neon para o PostgreSQL.
- **Auditei o próprio código antes de divulgá-lo** e encontrei a API sem regra de autorização
  e e-mails reais versionados no repositório. Fechei as rotas, habilitei a avaliação das
  anotações de autorização, movi a lista de administradores para variável de ambiente e
  reescrevi o histórico do Git.

`Java 21` `Spring Boot 3` `React` `PostgreSQL` `Google OAuth2`

<br>

## Stack

|  |  |
|---|---|
| **Backend** | ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white) ![Hibernate](https://img.shields.io/badge/JPA_/_Hibernate-59666C?style=flat-square&logo=hibernate&logoColor=white) ![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white) ![OAuth2](https://img.shields.io/badge/OAuth2-EB5424?style=flat-square&logo=auth0&logoColor=white) ![Swagger](https://img.shields.io/badge/OpenAPI-85EA2D?style=flat-square&logo=swagger&logoColor=black) |
| **Dados** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white) ![FalkorDB](https://img.shields.io/badge/FalkorDB-FF6B6B?style=flat-square) |
| **Testes** | ![JUnit5](https://img.shields.io/badge/JUnit_5-25A162?style=flat-square&logo=junit5&logoColor=white) ![Mockito](https://img.shields.io/badge/Mockito-78A641?style=flat-square) |
| **Frontend** | ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white) ![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white) |
| **Infra** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=black) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white) ![Neon](https://img.shields.io/badge/Neon-00E599?style=flat-square&logo=neon&logoColor=black) |
| **Práticas** | `Clean Code` `SOLID` `Arquitetura em camadas` `Multi-tenant` `Modelagem de dados` `LGPD` `Scrum` |

<br>

## Onde estou

**Estagiário de Suporte / TI** — UPCIGA Sistemas, remoto · desde jan/2026<br>
**Auxiliar Administrativo** — Monteiro Importados · desde dez/2023<br>
**Análise e Desenvolvimento de Sistemas** — IFPB, Campus Monteiro · conclusão prevista para jun/2027

<br>

<div align="center">
<sub>Aberto a oportunidades de <b>estágio ou júnior em backend</b>, com disponibilidade para trabalho remoto.</sub>
</div>
