# Padrões Arquiteturais

A arquitetura do sistema **LIVIA.us** foi estruturada com foco em modularidade, separação de responsabilidades e interoperabilidade entre sistemas e tecnologias diversas. Para isso, adotamos os padrões **Arquitetura em Camadas** e **Client-Server**, que juntos oferecem uma base sólida para desenvolvimento ágil, manutenção simplificada e escalabilidade da solução.

---

## 1. Arquitetura em Camadas

### O que é?
Arquitetura que divide o sistema em camadas bem definidas, onde cada uma possui responsabilidades específicas e interage apenas com suas camadas vizinhas. No **LIVIA.us**, temos:

- **Camada de Apresentação (Front-End):** Interface de usuário criada no Thunkable.
- **Camada de Negócio (Back-End):** Lógica de negócio implementada com Cloud Functions (Firebase).
- **Camada de Persistência (Banco de Dados):** Dados estruturados armazenados no Cloud Firestore.
- **Camada de Integração:** Comunicação com APIs e serviços externos (Firebase Auth, Google Maps API, Gov APIs, sistema de e-mail).

### Por que foi escolhida?

- **Organização e Clareza Arquitetural:** Separar as responsabilidades por camada facilita a leitura e manutenção do sistema.
- **Escalabilidade Modular:** As camadas podem evoluir de forma independente conforme as funcionalidades crescem.
- **Reutilização de Serviços:** O uso de APIs externas (como Google Maps e Firebase) permite concentrar a lógica interna apenas no necessário.
- **Testabilidade:** Cada camada pode ser testada isoladamente, garantindo maior qualidade do sistema.
- **Segurança e Controle de Fluxo:** A camada de autenticação e de lógica controla o que o usuário pode ou não acessar.

### Camadas no sistema

| Camada        | Tecnologias e Serviços                                 | Responsabilidade Principal                                                       |
|---------------|--------------------------------------------------------|-----------------------------------------------------------------------------------|
| Apresentação  | Thunkable                                              | Interface gráfica, telas, navegação e interação com o usuário final              |
| Negócio       | Cloud Functions (Firebase)                             | Processamento de lógica de negócios, controle de acesso e validação              |
| Persistência  | Cloud Firestore                                        | Armazenamento de UBSs, perfis, publicações, e dados estruturados                 |
| Integração    | Firebase Auth, Google Maps API, Gov APIs, E-mail       | Autenticação, geolocalização, busca de dados públicos, notificações, acessibilidade |

---

## 2. Arquitetura Client-Server

### O que é?
Um padrão arquitetural clássico em que os usuários (clientes) interagem com uma aplicação (servidor), que processa as requisições, executa a lógica e retorna dados. O cliente não armazena dados permanentes ou lógica de negócio pesada — essa responsabilidade é do servidor.

### Aplicação no LIVIA.us

- O **cliente** é o app mobile desenvolvido no Thunkable, que roda nos dispositivos dos usuários.
- O **servidor** é composto pelo backend em Cloud Functions e os serviços Firebase que executam e armazenam dados sob demanda.
- Comunicação entre cliente e servidor se dá via **requisições HTTPS** para autenticação, envio/consulta de publicações, localização de UBSs, entre outros.

### Por que foi escolhido?

- **Separação clara entre cliente e servidor:** Os dados e regras ficam no backend, o que melhora a segurança e facilita o controle de versões.
- **Desempenho leve no cliente:** O aplicativo é ágil mesmo em dispositivos com menos recursos.
- **Uso eficiente da nuvem:** Toda lógica é processada de forma serverless no Firebase, com escalabilidade automática.
- **Fácil manutenção:** Atualizações do servidor não exigem alterações no app instalado pelo usuário.

### Componentes Client-Server

| Entidade         | Papel no modelo Client-Server                                                  |
|------------------|---------------------------------------------------------------------------------|
| **Cliente (App)** | Interface usada por pacientes, visitantes, enfermeiros e usuários com acessibilidade |
| **Servidor**      | Firebase (Cloud Functions, Auth, Firestore) – executa a lógica e responde as solicitações |
| **Protocolos**    | Comunicação por HTTPS e APIs RESTful entre app e servidor                       |
