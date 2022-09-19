<span id="topo">

<h1 align="center">Sprint 1: 29/08/2022 a 18/09/2022</h1>

<p align="center">
    <a href="#objetivos">Objetivos da sprint</a> &nbsp |&nbsp &nbsp
    <a href="#entregas">Entregas</a> &nbsp |&nbsp &nbsp
    <a href="#metricas">Métricas do time</a> &nbsp |&nbsp &nbsp
    <a href="#links">Links úteis</a>
</p>

O projeto se baseia no desenvolvimento de um site para observação de dados meteorológicos, assim abrangendo a montagem e configuração de uma estação meteorológica com diversos tipos de sensores e um sistema capaz de ler os dados enviados por ela, permitindo a análise de seus dados em gráficos e tabelas tanto em modelo desktop/web quanto mobile. Tendo em mente o MVP, a primeira sprint se deu com a criação de telas e funcionalidades "chave", tais como fluxos de usuários (criação, exclusão e listagem), bem como de estações, om sua listagem e criação automática pelo backend. Para isso, foram levantados e validados os requisitos e o protótipo, construindo os serviços e interfaces visando uma entrega de grande valor condizente com os desejos do cliente.

<span id="objetivos">
    
## :dart: Objetivos da Sprint
Os requisitos (tanto do cliente como da instituição de ensino) abrangidos por essa sprint são:

- :heavy_check_mark: **RF 03:** Cadastro das estações, parâmetros e usuários
- :heavy_check_mark: **RF 05:** Dashboards para visualização dos parâmetros meteorológicos
- :heavy_check_mark: **RNF 08:** Implementar CI/CD
- :heavy_check_mark: **RNF 09:** Documentação

<span id="entregas">
        
## 🌤 Entregas
Para entregas da sprint, tivemos os artefatos SCRUM validados, como Backlog do Produto, Backlog das Sprints, Épicos e User Stories, através de comunicação direta entre o P.O. e o cliente. Para observar esses artefatos, acesse [este link](https://github.com/The-Bugger-Ducks/cloud-fox-documentation#backlogs).

Para extrair e entender os desejos do cliente, foi construído um protótipo inicial no Figma, criando a identidade visual e design do sistema e apresentando para validação com o cliente, onde o resultado deste protótipo foi traduzido para um site em React e com as devidas integrações das funcionalidades acordadas para esta sprint.

### ❄️ RF 03: Cadastro das estações, parâmetros e usuários

Este requisito se trata do cadastro de estações e usuários, o que significa permitir o CRUD completo de usuários além de criar, listar e acessar dados de estações. Para isso, foi desenvolvido o fluxo de usuários (desde login até exclusão de conta) e o dashboard de estações, porém, como o acordado entre time e cliente, o cadastro das estações será automático (entre a estação e o backend), sem parte interativa presente no frontend, mas sua automatização (do cadastro e recebimento dos dados de estações) serão desenvolvidos a partir da próxima sprint.

<div align="center">

| Fluxo de usuário comum                                                                                                | 
| :-------------------------------------------------------------------------------------------------------------------- |
| ![user_simple](https://user-images.githubusercontent.com/69374340/190942583-50d5ea43-d5a7-4ee2-a57c-7874c0b18f6d.gif) |

| Fluxo de usuário administrador                            |
| :-------------------------------------------------------- |
| ![user_admin](./user_admin.gif) |

| Fluxo de estações                  |
| :--------------------------------- |
| ![station](./station.gif) |

</div>

### 🌪 RF 05: Dashboards para visualização dos parâmetros meteorológicos

Este requisito se trata do modo de visualização dos dados emitidos pelas estações meteorológicas cadastradas. Na estrutura que foi implementada, qualquer usuário (fazendo login ou não, até o momento) pode acessar todos os dados disponíveis de estações existentes, como nome, localização e os dados enviados por seus sensores, observando-os em forma de gráficos de linha (onde o eixo horizontal é sempre o tempo e o vertical muda de unidade a cada tipo de sensor analisado, podendo representar milímetros de água, no caso do pluviômetro, graus Celsius, no caso do sensor de temperatura, entre outras unidades de medida possíveis).

<div align="center"><img src="https://user-images.githubusercontent.com/69374340/190942988-3b7975c7-95ab-4ff4-b2da-7840ffe30f0a.png" alt="Demonstração da dashboard de estações"></img></div>

### ☔️ RNF 08: Implementar CI/CD

Este requisito não funcional se trata da implementação de práticas de Integração e Entrega Contínua ("CI/CD") a pedido da FATEC. Prevê a aplicação de pipelines, realização de deploys, utilização de boas práticas com versionamento de código (como nomenclatura de branches, GitFlow, Conventional Commits, entre outros) além da criação de casos de teste que futuramente serão integrados ao sistema. Em relação a nomenclatura de branches é possível observar na documentação [desta tarefa](https://github.com/The-Bugger-Ducks/cloud-fox-documentation/issues/9), já os deploys se pode conferir pelos links abaixo:

- Backend: [https://cloud-fox.onrender.com/](https://cloud-fox.onrender.com/)
- Frontend: [https://cloud-fox.netlify.app/](https://cloud-fox.netlify.app/)

### ⚡️ RNF 09: Documentação

Este requisito se trata da criação de uma documentação acerca dos endpoints criados, seus parâmetros e retornos para facilitação do consumo da API e visibilidade das funcionalidades criadas. Para tal detalhamento foi utilizada a ferramenta [Swagger](https://swagger.io/), onde se pode realizar requisições e observar as rotas existentes através [deste link](https://cloud-fox.onrender.com/api-docs/#/).

→ [Voltar ao topo](#topo)

<span id="metricas">
    
## :chart_with_upwards_trend: Métricas do time
Em prol de um melhor aproveitamento das habilidades de cada integrante, o time foi separado em duas frentes: frontend e backend, onde, na primeira sprint, o time de frontend ficou responsável pela confecção do protótipo, projeto frontend e integração de funcionalidades enquanto o time de backend ficou responsável pela criação dos endpoints necessários e pesquisas sobre o tema do desafio, procurando implementar a melhor arquitetura possível. 
- O acompanhamento de atividades, de responsabilidade da Scrum Master, se encontra na imagem adiante, que contém o gráfico Burndown gerado pela equipe (onde o eixo X são os dias trabalhados na sprint e os valores do eixo Y representam as entregas e esforços realizados com o passar do tempo), incluindo as atividades desenvolvidas e seus responsáveis.
    
<div align="center">
    
![Burndown](https://user-images.githubusercontent.com/69374340/190932337-40f6e8a8-0b5c-4139-8083-0108c77fad6e.png)
</div>
    
<span id="links">
    
## :link: Links úteis

- Site do projeto: [https://cloud-fox.netlify.app/](https://cloud-fox.netlify.app/)
- Tags geradas em cada repositório que simbolizam o fim da 1ª sprint:
  - Repositório do site: [clique aqui para acessar "cloud-fox-web"](https://github.com/The-Bugger-Ducks/cloud-fox-web)
  - Repositório da API: [clique aqui para acessar "cloud-fox-back"](https://github.com/The-Bugger-Ducks/cloud-fox-back)

→ [Voltar ao topo](#topo)
