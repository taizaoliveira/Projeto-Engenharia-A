# Tech Stack Map

O mapa de tecnologias abaixo apresenta todas as ferramentas e serviços utilizados na construção do aplicativo **LIVIA.us**, organizados por camadas e responsabilidades dentro da arquitetura do sistema. A visualização permite compreender como cada tecnologia contribui para o funcionamento da solução e quais critérios justificam suas escolhas.

A estrutura segue uma abordagem modular, com camadas como **Front-End**, **Back-End**, **Banco de Dados**, **Autenticação**, **APIs**, **Modelagem e Design**, e **Gestão e Controle**, promovendo clareza, escalabilidade e facilidade de manutenção.

Cada tecnologia foi selecionada com base em critérios como:
- **Produtividade no desenvolvimento** (uso de plataformas no-code como Thunkable);
- **Integração nativa entre componentes** (como Firebase com Cloud Firestore e Auth);
- **Acessibilidade e inclusão** (uso de APIs nativas do dispositivo);
- **Suporte a funcionalidades essenciais** (como mapas e dados públicos via Google Maps API e GOV APIs);
- **Gerenciamento ágil de projeto** (Scrum, GitHub Projects).

Essa organização garante uma infraestrutura, adequada para o objetivo principal do sistema: conectar usuários e profissionais às Unidades Básicas de Saúde de forma georreferenciada, simples e inclusiva.

<p align="center">
  <img src="https://drive.google.com/uc?export=view&id=1th1nuxu0PGgp1U7aOLtmSRIjOzM7hLzi" />
</p>





## Mapa de Tecnologias

A definição do conjunto de tecnologias utilizadas no projeto **LIVIA.us** foi realizada com base nos objetivos do sistema: acessibilidade, rapidez no desenvolvimento, integração entre serviços e facilidade de manutenção.

Cada camada da arquitetura — do front-end até o gerenciamento do projeto — foi preenchida com ferramentas e plataformas específicas, escolhidas por sua compatibilidade, desempenho e facilidade de uso com as demais.

A tabela a seguir apresenta essas tecnologias organizadas por camada do sistema, explicando por que cada uma foi adotada. Esse mapeamento é fundamental para garantir rastreabilidade arquitetural, consistência técnica e clareza na evolução do sistema.


| Camada                 | Tecnologia                      | Justificativa                                                                                                                                                          |
|------------------------|----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Front-End              | Thunkable                        | Permite desenvolvimento rápido e multiplataforma (iOS/Android) sem a necessidade de código complexo, ideal para MVP e prototipagem ágil.                             |
|                        | APIs Nativas (GPS, Acessibilidade) | Essenciais para funcionalidades como geolocalização e inclusão digital. Thunkable permite uso direto dessas APIs nativas com acessibilidade por voz e leitura de tela. |
| Back-End               | Cloud Functions (Firebase)       | Execução de lógica de negócio de forma serverless, com escalabilidade automática e integração facilitada com bancos de dados, APIs externas e autenticação. Ideal para validar ideias rapidamente. |
| Banco de Dados         | Cloud Firestore                  | Banco NoSQL flexível e em tempo real, ideal para armazenar dados estruturados como UBSs, campanhas e perfis de usuários, com ótima integração ao Firebase e Thunkable. |
| Autenticação           | Firebase Auth                    | Gerenciamento completo de identidade (login, logout, redefinição de senha) com segurança embutida e fácil integração.                                                  |
| APIs                   | Google Maps API                  | Utilizada para exibir mapas, localização do usuário e das UBSs, com recursos de georreferenciamento. Essencial para a visualização espacial no app.                   |
|                        | GOV APIs                         | Fornecem dados públicos oficiais sobre Unidades Básicas de Saúde (UBSs), garantindo confiabilidade e atualização constante.                                           |
| Modelagem e Design     | Drawio                           | Usado para criação de diagramas de arquitetura (como C4), fluxogramas e representações estruturais do sistema.                                                         |
|                        | Figma                            | Ferramenta colaborativa de design de interfaces, prototipagem de telas e testes de usabilidade.                                                                       |
|                        | Canva                            | Suporte visual para criação de apresentações, identidade visual e materiais explicativos do projeto.                                                                  |
| Gestão e Controle      | Scrum                            | Metodologia ágil escolhida para organizar o trabalho em sprints, facilitando o acompanhamento de entregas e priorização de funcionalidades.                          |
|                        | GitHub + GitHub Projects         | Controle de versão, documentação do código e gerenciamento visual do backlog e progresso do projeto.                                                                  |
