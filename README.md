<span id="topo">

<h1 align="center">Sprint 2: 19/09/2022 a 09/10/2022</h1>

<p align="center">
    <a href="#objetivos">Objetivos da sprint</a> &nbsp |&nbsp &nbsp
    <a href="#entregas">Entregas</a> &nbsp |&nbsp &nbsp
    <a href="#metricas">Métricas do time</a> &nbsp |&nbsp &nbsp
    <a href="#links">Links úteis</a>
</p>

Nesta segunda sprint a equipe se voltou a atender os apontamentos sugeridos pelo cliente de refazer o modelo de dados empregado no projeto, além de precisar alterar a forma com que os dados são manipulados pela aplicação. Fora este retrabalho, foram desenvolvidos os requisitos acordados para esta sprint, como o início da criação do datalogger (que irá atuar na comunicação entre a estação meteorológica e o sistema) e cadastro de estações e seus sensores.

<span id="objetivos">
    
## :dart: Objetivos da Sprint
Os requisitos (tanto do cliente como da instituição de ensino) abrangidos por essa sprint são:

- :heavy_check_mark: **RF 01:** Criação de datalogger para uma estação meteorológica
- :heavy_check_mark: **RF 03:** Cadastro das estações, parâmetros e usuários
- :heavy_check_mark: **Requisitos não funcionais 08 e 09:** Implementar CI/CD e Documentação

<span id="entregas">
        
<br>
    
## 🌤 Entregas
Para esta entrega o foco se deu com o início da construção do datalogger para a estação meteorológica mas também a continuidade dos requisitos iniciados na primeira sprint, como o cadastro de estações, sensores e usuários além da implementação de CI/CD e documentação da API. Confira abaixo o resultado desta entrega:

### ❄️ RF 03: Criação de datalogger para uma estação meteorológica

Este requisito se trata do esboço da lógica que seria implantada no datalogger da estação meteorológica, esta que deve coletar e enviar informações a cerca de sensores para comunicação com nosso sistema, que por sua vez pode exibir os dados recebidos.

> 💡 Acesse o repositório com o código-fonte [neste link](https://github.com/The-Bugger-Ducks/cloud-fox-iot)

### ❄️ RF 03: Cadastro das estações, parâmetros e usuários

Tal requisito, iniciado na sprint passada, agora engloba formulários para criação de estações e seus sensores.

<div align="center">

| Cadastro de estações e seus sensores                       |
| :--------------------------------------------------------: |
| ![Demonstração do cadastro de estações](./new_station.gif) |

</div>
    
### ❄️ RF 05: Dashboards para visualização dos parâmetros meteorológicos

Atendendo a pedidos do cliente para agregar mais dinamismo ao banco de dados da aplicação, todo o modelo de dados foi reformulado ao que se diz respeito a estações, seus sensores e as coletas de dados propriamente ditas. Abaixo se pode observar o modelo utilizado na primeira sprint, que para os requisitos iniciais não revelou grandes problemas, mas que limitava o sistema o suficiente para que uma revisão fosse necessária (imagem da esquerda), e o novo modelo implementado que abrange muito mais possibilidades a cerca de sensores (imagem da direita)

<details>
    <summary><b>Comparação do modelo de dados</b></summary>
<div align="center">

| Antes                                      | Depois                                     |
| :----------------------------------------: | :----------------------------------------: |
| ![Antes](https://user-images.githubusercontent.com/69374340/194787430-d8a63838-fa40-4b9c-a918-12963190c15a.png) |![Depois](https://user-images.githubusercontent.com/69374340/194787433-fb8eb5af-5c60-4481-a4b5-5389f5d39f86.png) |

</div>
</details>
        
<br>
    
<span id="metricas">
    
## :chart_with_upwards_trend: Métricas do time
Em prol de um melhor aproveitamento das habilidades de cada integrante, o time foi separado em duas frentes: frontend e backend, onde, nesta sprint, o time de frontend ficou responsável pela confecção dos formulários de criação de estações e sensores, além de refatorações na manipulação dos dados de coletas, enquanto o time de backend ficou responsável pela "remodelagem" do banco de dados e endpoints afetados, bem como a criação do datalogger. 
- O acompanhamento de atividades, de responsabilidade da Scrum Master, se encontra na imagem adiante, que contém o gráfico Burndown gerado pela equipe (onde o eixo X são os dias trabalhados na sprint e os valores do eixo Y representam as entregas e esforços realizados com o passar do tempo), incluindo as atividades desenvolvidas e seus responsáveis.
    
<div align="center">
    
![Gráfico de Burndown](https://user-images.githubusercontent.com/69374340/194781689-c64faf6c-4ecf-4abb-b8c1-60799196473c.png)
</div>
    
            
<br>
    
<span id="links">
    
## :link: Links úteis

- Site do projeto: [https://cloud-fox.netlify.app/](https://cloud-fox.netlify.app/)
- Tags geradas em cada repositório que simbolizam o fim da 2ª sprint:
  - Repositório do site: [clique aqui para acessar "cloud-fox-web"](https://github.com/The-Bugger-Ducks/cloud-fox-web)
  - Repositório da API: [clique aqui para acessar "cloud-fox-back"](https://github.com/The-Bugger-Ducks/cloud-fox-back)
  - Repositório do Datalogger: [clique aqui para acessar "cloud-fox-iot"](https://github.com/The-Bugger-Ducks/cloud-fox-iot)

→ [Voltar ao topo](#topo)
