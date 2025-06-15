# 📋 PLANO DE TRABALHO

|                         |                                                                                                                                            |
|-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Nome do Projeto:**              | Aplicativo de Localização Integrado para Visualização de Informações e Acesso às Unidades de Saúde de Itacoatiara - AM.      |
| **Codinome:**                       | LIVIA.us                                                             |
| **Versão:**                       | 1.4                                                              |
| **Status:**                       | Em desenvolvimento                                               |
| **Número de Controle SRBR-M:**    | SRBR-M-001                                     |
| **Executor Principal:**           | Bugs Squad                                                 |
| **Coordenador do Projeto:**       | Prof. Dr. Andrey Rodrigues                                        |


---

## 📜 HISTÓRICO DE VERSÕES

| Versão | Descrição                | Autor   | Data   |
|--------|--------------------------|---------|--------|
| 1.0    | Elaboração do Plano Inicial     | Taíza  | 09/04/2025  |
| 1.1    | Revisão e ajustes no Plano Inicial     | Taíza  | 12/04/2025  |
| 1.2    | Atualização do Plano Inicial com novas informações e ajustes    | Taíza  | 15/04/2025  |
| 1.3    | Revisão eAtualização do Plano com inclusão de novas informações e ajustes finais    | Taíza  | 12/05/2025  |
| 1.4    | Inclusão da seção de Arquitetura do Sistema, com definição de padrão arquitetural, mapa de tecnologias, representação em múltiplos níveis segundo o modelo C4 (contexto, containers, componentes e código), e rastreabilidade com histórias do usuário. | Taíza | 15/06/2025 |

---

## 📑 ÍNDICE

1. [INTRODUÇÃO](#1-introdução)  
   1.1 [Objeto](#11-objeto)  
   1.2 [Motivação, Justificativa e Oportunidade](#12-motivação-justificativa-e-oportunidade)  
   1.3 [Caracterização do Projeto](#13-caracterização-do-projeto)  
   &nbsp;&nbsp;&nbsp;&nbsp;1.3.1 [Classe](#131-classe)  
   &nbsp;&nbsp;&nbsp;&nbsp;1.3.2 [Enquadrabilidade](#132-enquadrabilidade)  
   &nbsp;&nbsp;&nbsp;&nbsp;1.3.3 [Tipo](#133-tipo)  

2. [INFORMAÇÕES GERAIS](#2-informações-gerais)  
   2.1 [Escopo Geral](#21-escopo-geral)  
   &nbsp;&nbsp;&nbsp;&nbsp;2.1.1 [Escopo Específico](#211-escopo-específico)  
   &nbsp;&nbsp;&nbsp;&nbsp;2.1.2 [Escopo Negativo](#212-escopo-negativo)  
   2.2 [Ambiente de Desenvolvimento](#22-ambiente-de-desenvolvimento)  
   2.3 [Características Inovadoras do Projeto](#23-características-inovadoras-do-projeto)  
   2.4 [Resultados Esperados](#24-resultados-esperados)  

3. [METODOLOGIA DE PROJETO](#3-metodologia-de-projeto)  
   3.1 [Estrutura do Projeto](#31-estrutura-do-projeto)  
   3.2 [Equipe de Projeto: Papéis e Responsabilidades dos integrantes](#32-equipe-de-projeto-papéis-e-responsabilidades-dos-integrantes)  
   3.3 [Backlog do Sprint](#33-backlog-do-sprint)  
   3.4 [Controle de Mudanças](#34-controle-de-mudanças)  
   3.5 [Gerenciamento de Comunicação](#35-gerenciamento-de-comunicação)  


   

---

## 1. INTRODUÇÃO

### 1.1 Objeto
O projeto tem como objetivo desenvolver um aplicativo móvel gratuito e acessível para ajudar os usuários a localizar as Unidades Básicas de Saúde (UBSs) na cidade de Itacoatiara. O app também mostrará as áreas de atendimento de cada unidade, oferecerá conteúdos informativos sobre saúde por meio de publicações e contará com um canal de atendimento via chat. Além disso, a plataforma incluirá recursos de acessibilidade e perfis personalizados para melhor atender às necessidades dos usuários.

### 1.2 Motivação, Justificativa e Oportunidade
A criação de um aplicativo móvel gratuito e acessível para localizar Unidades Básicas de Saúde (UBSs) em Itacoatiara surge da necessidade de facilitar o acesso da população aos serviços de saúde pública, especialmente em regiões com limitações de informação e mobilidade. A iniciativa é motivada pela carência de uma ferramenta digital centralizada que informe, de forma clara e acessível, sobre as áreas de atendimento de cada UBS, seus serviços e localização. Justifica-se, portanto, a importância de promover inclusão digital e social, oferecendo também conteúdos informativos sobre saúde, canal de atendimento via chat e recursos de acessibilidade que contemplam diferentes perfis de usuários. Essa proposta representa uma oportunidade de fortalecer a relação entre população e sistema de saúde, contribuindo para a melhoria da qualidade do atendimento e da disseminação de informações essenciais à promoção da saúde.

### 1.3 Caracterização do Projeto

#### 1.3.1 Classe
| Classe             | Detalhamento                                                         |
|--------------------|----------------------------------------------------------------------|
| Aplicativo Móvel   | Aplicativo gratuito e acessível voltado para dispositivos móveis, desenvolvido para auxiliar a população de Itacoatiara na localização das UBSs e no acesso a informações de saúde. Conta com mapa interativo com áreas de atendimento, publicações educativas, canal de atendimento via chat e recursos de acessibilidade para diferentes perfis de usuários.    |

#### 1.3.2 Enquadrabilidade
| Enquadrabilidade    | Detalhamento                                                      |
|---------------------|-------------------------------------------------------------------|
| Software de Interesse Social | O aplicativo promove a inclusão digital e o acesso à informação em saúde, atendendo populações com baixa conectividade e mobilidade reduzida.   |
| Aplicativo de Utilidade Pública | Destinado ao uso da população em geral para facilitar a localização de unidades de saúde e acesso a conteúdos informativos sobre cuidados com a saúde. |
| Tecnologias Assistivas     | Inclui funcionalidades de acessibilidade, como leitor de tela, design responsivo e navegação simplificada, promovendo o acesso de pessoas com deficiência. |

#### 1.3.3 Tipo
| Tipo                  | Detalhamento                                                                 |
|-----------------------|------------------------------------------------------------------------------|
| Desenvolvimento         | Construção de um aplicativo móvel com funcionalidades voltadas para a realidade local.           |
| Trabalho Acadêmico      | Projeto desenvolvido no contexto da disciplina de Engenharia de Software I como proposta prática. |
| Projeto de Impacto Social | Voltado à solução de problemas enfrentados pela população de Itacoatiara no acesso à saúde.   |

---

## 2. INFORMAÇÕES GERAIS

### 2.1 Escopo Geral
Desenvolver um aplicativo móvel gratuito com foco na saúde pública, voltado para facilitar o acesso da população de Itacoatiara às Unidades Básicas de Saúde (UBSs). A solução visa centralizar informações essenciais sobre localização, área de cobertura por bairro, campanhas e eventos locais, além de oferecer recursos de acessibilidade e um canal direto de comunicação com as unidades. O aplicativo será intuitivo, leve e permitirá a navegação básica sem necessidade de login.

### 2.1.1 Escopo Específico
- Georreferenciamento das UBSs da cidade.
- Visualização da área de cobertura de cada UBS, segmentada por bairros.
- Feed com campanhas, ações de saúde e eventos por unidade.
- Canal de atendimento via chat com informações sobre funcionamento, serviços e horários.
- Navegação no modo visitante (sem necessidade de login).
- Funcionalidades de acessibilidade (voz e leitura de tela). 

### 2.1.2 Escopo Negativo
- O aplicativo não permitirá agendamento de consultas médicas.
- Não terá integração com redes sociais ou autenticação por terceiros.
- Não incluirá funcionalidades de triagem ou diagnósticos automatizados com base em sintomas.

### 2.2 Ambiente de Desenvolvimento

| Componente             | Tecnologia/Ferramenta                     |
|------------------------|-------------------------------------------|
| Metodologia            | Scrum com sprints                         |
| Gerenciamento de Backlog | GitHub Projects                                 |
| Repositório de Código  | GitHub                                   |
| Modelagem de Software  | Draw.io, Figma, Canva, PowerPoint                  |
| Desenvolvimento do MVP | Thunkable, Firebase                 |

### 2.3 Características Inovadoras do Projeto
- Mapeamento detalhado das UBSs com visualização clara de áreas de abrangência por bairro.
- Feed informativo e atualizado com campanhas de vacinação, eventos e ações comunitárias.
- Acessibilidade por voz e leitura de tela integrada desde a primeira tela.
- Chat com dúvidas frequentes sobre horários e serviços disponíveis.
- Uso sem login obrigatório, promovendo inclusão digital e facilidade de acesso. 

### 2.4 Resultados Esperados
- Um aplicativo funcional que localiza e descreve UBSs com base na localização do usuário.
- Visualização da área de atuação de cada UBS, com filtros por bairro.
- Feed ativo com conteúdos locais relevantes, campanhas e eventos.
- Canal de dúvidas via chat, com respostas básicas e direcionamento.
- Aplicativo acessível e leve, com uso descomplicado, inclusive por idosos ou pessoas com deficiência.
- Repositório GitHub com documentação, Notion e versão navegável do app 

---

## 3. METODOLOGIA DE PROJETO

### 3.1 Estrutura do Projeto  
O desenvolvimento do aplicativo será dividido em fases estratégicas, cada uma com etapas específicas que visam garantir clareza, alinhamento com as necessidades dos usuários e viabilidade técnica da solução.  
**Fases:**  
#### 1. **Conceito/Ideia**
#### **Definição do problema**   
A população em geral, especialmente em regiões periféricas e com menor acesso à informação digital, enfrenta dificuldades para acessar serviços essenciais de saúde pública devido à falta de comunicação clara, centralizada e acessível sobre o funcionamento das Unidades Básicas de Saúde (UBSs). Muitas pessoas não sabem qual unidade devem procurar, desconhecem os serviços disponíveis, e não têm acesso a informações sobre campanhas, eventos e ações de saúde promovidas em suas comunidades. Essa lacuna de informação reduz o engajamento da população com a atenção primária à saúde, sobrecarrega outros níveis de atendimento (como UPAs e hospitais) e compromete a eficácia das políticas públicas de prevenção. O aplicativo LIVIA.us surge como resposta a esse cenário, buscando aproximar a população dos serviços públicos de saúde por meio de uma plataforma acessível, intuitiva e centrada nas necessidades reais dos usuários.   
🔗 [Acessar o Enquadramento do Problema](https://github.com/taizaoliveira/Projeto-Engenharia-A/blob/main/SPRINT%201/2%20-%20Design%20Thinking/FASE%20I%20-%20INSPIRA%C3%87%C3%83O/1.%20Enquadramento%20do%20Problema%20-%20Golden%20Circle.md)   
    
#### **Análise de concorrentes**    
O projeto "LIVIA.us" se diferencia por focar exclusivamente nas UBS e na inclusão digital, mas enfrenta concorrência de soluções já implementadas no setor público de saúde. Entre os principais concorrentes estão:    
- Mais Saúde Fortaleza: App da Prefeitura de Fortaleza com foco em serviços de saúde, como agendamentos, localização de postos e lembretes de vacinação.
- e-saudeSP: Plataforma integrada da Prefeitura de São Paulo com IA para triagem, dados unificados do paciente e localização de UBS e farmácias.
- Google Maps: Embora não voltado à saúde, é amplamente utilizado para localização de unidades, com rotas, avaliações e integração com estabelecimentos.  
  
🔗 [Acessar a Exploração de Mercado](https://github.com/taizaoliveira/Projeto-Engenharia-A/blob/main/SPRINT%201/2%20-%20Design%20Thinking/FASE%20I%20-%20INSPIRA%C3%87%C3%83O/2.%20Explora%C3%A7%C3%A3o%20do%20Mercado.md)    
    
#### **Identificação de diferenciais**    
A Tabela abaixo apresenta um quadro comparativo entre soluções digitais voltadas à área da saúde e serviços geolocalizados, com o objetivo de evidenciar os principais diferenciais da proposta aqui desenvolvida — o aplicativo LIVIA.us. Nota-se que, embora existam aplicações amplamente utilizadas como o Mais Saúde Fortaleza, o e-saudeSP e até mesmo o Google Maps, estas apresentam limitações quanto à adaptação ao contexto local, acessibilidade integral e vínculo com as unidades de saúde de base comunitária.     
Neste cenário, o LIVIA.us se destaca por seu enfoque territorial na cidade de Itacoatiara (AM), pela utilização de tecnologias acessíveis e de baixo custo, e pelo compromisso com a inclusão digital e a acessibilidade, ao incorporar funcionalidades como leitores de tela e conexão direta com Unidades Básicas de Saúde (UBS).   
  
<p align="center">
  <img src="https://drive.google.com/uc?export=view&id=1Wi4cwYJDmGM6BpviyBX9OfVaYkaM5kvJ" height="600"  width="800"/>
</p>


   
#### **Perfis de usuários**   
Com base na abordagem de design centrado no ser humano, foram definidas quatro personas para orientar o desenvolvimento funcional e inclusivo do aplicativo LIVIA.us, considerando o contexto socioeconômico e os padrões de uso da população de Itacoatiara (AM).
- Usuário Cadastrado: representa o cidadão que utiliza o aplicativo de forma recorrente, com conta ativa. Este perfil possui acesso ampliado às funcionalidades do sistema, incluindo chat com profissionais de saúde. Trata-se de um usuário engajado, interessado em manter-se informado sobre a saúde pública local e em dialogar com a rede de atenção básica.
- Visitante: caracteriza o usuário eventual, que navega no aplicativo sem a necessidade de login. Tem acesso apenas às funcionalidades básicas, como a visualização de UBS próximas, horários de funcionamento e localização. Não possui acesso ao chat, priorizando uma experiência rápida, leve e eficiente, mesmo em situações de conectividade limitada.
- Enfermeiro: corresponde ao profissional da área da saúde que utiliza o app como ferramenta de apoio à comunicação com a comunidade. Atua na atualização de informações locais e no atendimento via chat, representando o elo direto entre a atenção básica e os cidadãos cadastrados.
- Usuário com Necessidades de Acessibilidade: abrange indivíduos com deficiência visual, auditiva ou motora. Este perfil é contemplado com funcionalidades como leitura de tela, comandos por voz, botões ampliados e interface simplificada, reforçando o compromisso do projeto com a inclusão digital e o acesso equitativo à saúde..

🔗 [Acessar as Personas do Projeto ](https://github.com/taizaoliveira/Projeto-Engenharia-A/blob/main/SPRINT%201/2%20-%20Design%20Thinking/FASE%20I%20-%20INSPIRA%C3%87%C3%83O/3.%20Conhecendo%20o%20usu%C3%A1rio%20-%20Persona.md)   

#### 2. **Levantamento de Requisitos**  
A fase de levantamento e especificação de requisitos teve como objetivo identificar, organizar e validar as funcionalidades essenciais para o desenvolvimento do aplicativo LIVIA.us, garantindo alinhamento com as necessidades reais dos usuários e com os objetivos do projeto. Foram adotadas práticas de Engenharia de Requisitos centradas no usuário, com base em entrevistas, definição de personas, estudo de campo e priorização contínua por meio de backlog refinado.  
O processo incluiu:  
- Levantamento de Requisitos: identificação inicial de funcionalidades e restrições do sistema, considerando aspectos técnicos, sociais e contextuais da cidade de Itacoatiara.
- Refinamento do Backlog: organização iterativa e incremental das funcionalidades, utilizando critérios de prioridade, valor social e viabilidade técnica.
- Critérios de Aceitação: definição objetiva de condições mínimas para considerar uma funcionalidade como "pronta", garantindo clareza e qualidade nas entregas.
- Regras de Negócio: descrição das normas, restrições e comportamentos esperados no sistema, de acordo com os fluxos reais das unidades de saúde e o perfil dos usuários.    
  
🔗 [Detalhamento da Fase de Requisitos ](https://github.com/users/taizaoliveira/projects/2)  

### 3. **Projeto e Arquitetura**  
#### Modelagem de telas e navegação  
`Em desenvolvimento ...`  

#### Arquitetura do sistema  
Esta etapa tem como objetivo planejar, representar e justificar a arquitetura da solução proposta, garantindo rastreabilidade com as histórias de usuário e alinhamento com os requisitos do sistema. A documentação foi organizada de forma modular, seguindo boas práticas e baseada no modelo C4.

##### 🔹 Definição do Padrão Arquitetural
Escolha e justificativa dos padrões arquiteturais utilizados, com base nos requisitos e nos objetivos do sistema.  
📄 Arquivo: [`Padrao_Arquitetural.md`](https://github.com/taizaoliveira/Projeto-Engenharia-A/blob/main/SPRINT%202/Arquitetura%20do%20Software/1%20-%20Padr%C3%A3o%20Arquitetural/Padrao_Arquitetural.md) 

---

##### 🔹 Mapa de Tecnologias (Tech Stack)
Mapeamento das tecnologias utilizadas organizadas por camada (frontend, backend, banco de dados etc.), incluindo justificativas.  
📄 Arquivo: [`Tecnologias_e_Ferramentas.md`](https://github.com/taizaoliveira/Projeto-Engenharia-A/blob/main/SPRINT%202/Arquitetura%20do%20Software/2%20-%20Tecnologias%20e%20Ferramentas/Tecnologias_e_Ferramentas.md) 

---

##### 🔹 Modelo C4 – Representação Arquitetural
Representação da arquitetura do sistema em diferentes níveis de abstração:

- **Diagrama de Contexto:** Atores e sistemas externos  
  📄 [`1_Diagrama_de_Contexto.md`](https://github.com/taizaoliveira/Projeto-Engenharia-A/blob/main/SPRINT%202/Arquitetura%20do%20Software/3%20-%20Arquitetura%20Modelo%20C4/1_Diagrama_de_Contexto.md) 

- **Diagrama de Containers:** Blocos de execução, linguagens e comunicação  
  📄 [`2_Diagrama_de_Containers.md`](https://github.com/taizaoliveira/Projeto-Engenharia-A/blob/main/SPRINT%202/Arquitetura%20do%20Software/3%20-%20Arquitetura%20Modelo%20C4/2_Diagrama_de_Containers.md)

- **Diagrama de Componentes:** Serviços, controladores, repositórios e lógica interna  
  📄 [`3_Diagrama_de_Componentes.md`](https://github.com/taizaoliveira/Projeto-Engenharia-A/blob/main/SPRINT%202/Arquitetura%20do%20Software/3%20-%20Arquitetura%20Modelo%20C4/3_Diagrama_de_Componentes.md)

- **Diagrama de Código:** UML com classes, métodos e atributos  
  📄 [`4_Diagrama_de_Código.md`](https://github.com/taizaoliveira/Projeto-Engenharia-A/blob/main/SPRINT%202/Arquitetura%20do%20Software/3%20-%20Arquitetura%20Modelo%20C4/4_Diagrama_de_C%C3%B3digo.md)

---

##### 🔹 Rastreabilidade com Histórias do Usuário
Mapeamento entre as histórias do usuário e os componentes do sistema, indicando onde aparecem nos diagramas arquiteturais.  
📄 Arquivo: [`Rastreabilidade_Historia_Usuario.md`](https://github.com/taizaoliveira/Projeto-Engenharia-A/blob/main/SPRINT%202/Arquitetura%20do%20Software/4%20-%20Rastreabilidade%20Com%20Hist%C3%B3rias%20do%20Usu%C3%A1rio/Rastreabilidade_Historia_Usuario.md)

#### Diagramas de classes  
`Em desenvolvimento ...`  

#### Prioridades para o MVP  
`Em desenvolvimento ...`  

#### 4. **Projeto dos Casos de Teste**  
   - Cenários de teste `Em desenvolvimento ...`   
   - Casos baseados em histórias de usuário  `Em desenvolvimento ...`
   - Critérios de sucesso  `Em desenvolvimento ...`

#### 5. **Desenvolvimento do MVP**  
   - Implementação no framework X  `Em desenvolvimento ...`
   - Testes e ajustes iterativos  `Em desenvolvimento ...`
   - Apresentação e validação  `Em desenvolvimento ...`

### 3.2 Equipe de Projeto: Papéis e Responsabilidades dos integrantes

| Papel            | Responsabilidades                                                  |
|------------------|--------------------------------------------------------------------|
| Andrey Rodrigues    |                  Product Owner (PO)                                                  |
| Brayner Santana    |                  QA / Testes                                                  |
| Gabriela Rodrigues    |                  QA / Testes                                                  |
| Gregory Ozaki    |                  UX/UI Designer                                                   |
| Leano Baba    |                  Dev Backend                                                  |
| Taíza Paula    |                  Scrum Master e Dev Mobile                                                  |

### 3.3 Backlog do Sprint
O desenvolvimento do aplicativo LIVIA.us é conduzido de forma incremental, com uso de Sprints semanais organizadas no GitHub Projects. O backlog do sprint é derivado do backlog do produto e contém as tarefas comprometidas para o ciclo atual, priorizadas com base no valor para o usuário e na viabilidade técnica.  
As tarefas estão categorizadas por fase do projeto — Backlog, Em progresso e Concluídas — o que permite uma visualização clara do progresso e facilita o acompanhamento por toda a equipe.  
O planejamento semanal é orientado por reuniões de alinhamento e revisões periódicas, assegurando a adaptação contínua às demandas do projeto.

🔗 [Backlog do Sprint 1](https://github.com/users/taizaoliveira/projects/5/views/1)  
🔗 [Backlog do Sprint 2](https://github.com/users/taizaoliveira/projects/8/views/1)  

### 3.4 Controle de Mudanças
O controle de mudanças no projeto LIVIA.us é realizado de forma estruturada, visando garantir a rastreabilidade, a organização e a validação coletiva das alterações propostas. Qualquer modificação no escopo, funcionalidades ou prioridades do backlog deve ser formalizada por meio de GitHub Issues, onde a proposta é documentada, justificada e discutida.  
As mudanças são avaliadas durante a reunião de planejamento semanal, momento em que a equipe decide, de forma colaborativa, sobre a aceitação, priorização ou replanejamento das tarefas impactadas. Essa abordagem assegura transparência, controle e alinhamento contínuo com os objetivos do projeto e as necessidades dos usuários.
  
🔗 [Mudanças via GitHub Issues ](https://github.com/taizaoliveira/Projeto-Engenharia-A/issues?q=is%3Aissue%20state%3Aopen)  

### 3.5 Gerenciamento de Comunicação
O gerenciamento de comunicação no projeto LIVIA.us é essencial para garantir a colaboração eficiente entre os membros da equipe, promovendo transparência, alinhamento e agilidade nas decisões. Foram definidas rotinas fixas de comunicação, bem como o uso de ferramentas colaborativas que facilitam o acompanhamento das atividades e o registro de decisões.  
As práticas de comunicação seguem os princípios das metodologias ágeis, com rituais semanais e diários conforme a tabela a seguir:

O gerenciamento de comunicação no projeto **LIVIA.us** foi estruturado para garantir alinhamento constante entre os membros da equipe, utilizando práticas ágeis e ferramentas colaborativas. Abaixo, detalhamos os principais rituais e canais adotados:

####  Práticas de Comunicação

|       **Práticas**               | **Frequência**     | **Horário** | **Formato**                        | **Objetivo**                                                  |
|----------------------------------|--------------------|-------------|------------------------------------|---------------------------------------------------------------|
| Sprint Planning                  | Semanal (segunda)  | 13h         | Google Meet ou presencial          | Planejamento e definição das tarefas da sprint                |
| Daily Stand-up                   | Diária             | 9h          | Formulário (Google Forms + Notion) | Compartilhamento de progresso, bloqueios e próximos passos    |
| Retrospective | Semanal (sexta) | 13h | Google Meet ou Presencial | Apresentação de entregas, feedbacks e melhorias continuas |
| Sprint Review    | Mensal    | 20h às 22h         | Presencial com PO                      | Apresentação de entregas, feedbacks e melhorias contínuas     |

#### 🛠️ Ferramentas Utilizadas

- **WhatsApp**: Comunicação rápida e informal da equipe
- **Notion**: Registro de dailies, documentos e decisões
- **GitHub**: Controle de versões, issues e organização de sprints
- **Google Drive**: Armazenamento e compartilhamento de arquivos



