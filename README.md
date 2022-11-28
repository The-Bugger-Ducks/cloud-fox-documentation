<span id="topo">

<h1 align="center">Sprint 4: 07/11/2022 a 27/11/2022</h1>

<p align="center">
    <a href="#objetivos">Objetivos da sprint</a> &nbsp |&nbsp &nbsp
    <a href="#entregas">Entregas</a> &nbsp |&nbsp &nbsp
    <a href="#metricas">Métricas do time</a> &nbsp |&nbsp &nbsp
    <a href="#links">Links úteis</a>
</p>

Para a última sprint a equipe desenvolveu os requisitos planejados além de aplicar
melhorias visando melhorias na usabilidade do sistema (como por exemplo a
implementação de notificações personalizadas ao invés do uso dos alertas padrão do
navegador). Com isso, é tido como entregável desta sprint o sistema com todas as
funcionalidades iniciais satisfeitas, desde a montagem da estação (com apoio das aulas
de IoT), programação do datalogger (para gerenciar e enviar os dados das coletas), sistema
receptor e processador das coletas e uma plataforma para visualização dos dados (que pode
ser acessada pelo seguinte endereço: [cloud-fox.netlify.app](https://cloud-fox.netlify.app/))

<span id="objetivos">
    
## :dart: Objetivos da Sprint
Os requisitos (tanto do cliente como da instituição de ensino) abrangidos por essa sprint são:

- :heavy_check_mark: **RF 02:** Montagem de uma estação meteorológica
- :heavy_check_mark: **RF 07:** Geração de alertas
- :heavy_check_mark: **RNF 06:** Tutorial do significado de cada parâmetro meteorológico

<span id="entregas">
        
## 🌤 Entregas
Focados em concluir os requisitos restantes, o grupo voltou-se a pesquisas, questionamentos ao cliente e muito planejamento para modelar uma solução plausível aos problemas apresentados, resultando nas seguintes entregas:

### 🌪 RF 02: Montagem de uma estação meteorológica

Este requisito se trata da criação de uma estação meteorológica que contém vários tipos de sensores como de temperatura, umidade e pluviômetro. Conforme o acompanhamento das aulas de IoT que serviram de base para a conclusão desse requisito, é possível observar o resultado através da utilização do datalogger associado aos sensores, que assim que identifica os sensores já inicia o envio dos dados a cada 1 hora, dados esses que são recebidos e armazenados pelo sistema, disponível então para visualização dos mesmos na plataforma.

> Para analisar o código fonte do datalogger acesse [cloud-fox-iot](https://github.com/The-Bugger-Ducks/cloud-fox-iot).

### ⚡️ RF 07: Geração de alertas

Tal requisito se trata da possibilidade de criar alertas que relacionam um parâmetro meteorológico a um determinado limite, seja mínimo ou máximo, assim, caso os valores lidos ultrapassem esta faixa, um alerta é gerado e adicionado ao status da estação, que agrupa o estado de cada alerta cadastrado (podendo variar entre "verde", "amarelo" ou "vermelho" a partir da relação entre valor e limite estabelecido). O cadastro de alertas pode ser feito por administradores e gerenciadores de estação pela dashboard de cada estação, e a sua visualização é feita a partir da mesma página, pelo ícone de alerta no canto superior direito, vide demonstração:

<div align="center">

![Demonstração da geração de alertas]()

</div>

> **Observação:** devido a complexidade deste requisito a nível estrutural (criar o modelo do banco de dados, os endpoints e a integração do serviço), a entrega está sendo feita através das funcionalidades "mockadas", onde não há real interação entre frontend e backend, logo, não há armazenamento de novos alertas.

### ☔️ RNF 06: Tutorial do significado de cada parâmetro meteorológico

Este requisito não funcional se trata da criação de tutoriais para explanação dos significados dos parâmetros meteorológicos manipulados visando auxiliar no aprendizado, entendimento e interpretação dos dados apresentados na plataforma em forma de gráficos. Essa explicação foi adicionada à plataforma por meio da criação de uma nova página no sistema, contendo informações interessantes sobre os parâmetros e dados analisados, relacionando áreas de conhecimento (como física ou matemática) à fórmulas e usabilidades.

<div align="center">

![Demonstração do tutorial](https://user-images.githubusercontent.com/69374340/204171167-15ad6e09-30c9-4e6b-bad2-59d44d4508ec.png)

</div>

### ✨ Melhorias gerais

- [ ] **Deploy na AWS:** iniciada na sprint anterior esta tarefa se deu com a aplicação de muitos esforços em configurar um ambiente propício para a execução da plataforma como um todo (frontend e backend integrados), porém, devido a diversas dificuldades encontradas e a falta de direcionamento e experiência, sua conclusão não foi possível.
- [x] **Toasts (notificações):** com a proposta de melhorar a experiência dos usuários, os alertas (antes empregados utilizando o estilo de alerta padrão emitido pelo navegador) foram atualizados para notificações personalizadas no interior da página, trazendo assim mais fluidez no uso do sistema e tornando a interface dos alertas mais agradável.

<div align="center">

![Demonstração das notificações]()

</div>

→ [Voltar ao topo](#topo)

<span id="metricas">
    
## :chart_with_upwards_trend: Métricas do time
Em prol de um melhor aproveitamento das habilidades de cada integrante, o time foi separado em duas frentes: frontend e backend, onde o "time front" focou no desenvolvimento das interfaces para cadastro e exibição de alertas das estações além de realizar ajustes como a alteração das notificações de alerta do sistema. Já o "time back" atuou em melhorias do datalogger, montagem da estação e criação dos serviços necessários para a criação e exibição dos alertas das estações, além de depositar grandes esforços em melhorias do deploy. 
- O acompanhamento de atividades, de responsabilidade da Scrum Master, se encontra na imagem adiante, que contém o gráfico Burndown gerado pela equipe (onde o eixo X são os dias trabalhados na sprint e os valores do eixo Y representam as entregas e esforços realizados com o passar do tempo), incluindo as atividades desenvolvidas e seus 
responsáveis.
    
<div align="center">

![Burndown](https://user-images.githubusercontent.com/69374340/204172089-75daeed0-a581-4395-918e-c6ffc4f5d1ce.png)

</div>

<details>
 <summary>Lista de atividades desenvolvidas (com estimativa, responsável e datas)</summary>
 <br>
<div align="center">
 
![Tarefas](https://user-images.githubusercontent.com/69374340/204172182-67792b8a-edef-480a-ab4c-b69d04f9ce8d.png)
</div>

</details>
    
<span id="links">
    
## :link: Links úteis

- Site do projeto: [https://cloud-fox.netlify.app/](https://cloud-fox.netlify.app/)
- Tags geradas em cada repositório que simbolizam o fim da 3ª sprint:
  - Repositório do site: [clique aqui para acessar "cloud-fox-web"](https://github.com/The-Bugger-Ducks/cloud-fox-web)
  - Repositório da API: [clique aqui para acessar "cloud-fox-back"](https://github.com/The-Bugger-Ducks/cloud-fox-back)
  - Repositório do datalogger: [clique aqui para acessar "cloud-fox-iot"](https://github.com/The-Bugger-Ducks/cloud-fox-iot)

→ [Voltar ao topo](#topo)
