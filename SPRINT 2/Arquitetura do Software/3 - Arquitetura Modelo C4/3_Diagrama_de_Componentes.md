# Diagrama de Componentes

O diagrama de componentes detalha os módulos internos de cada container do sistema. Ele representa serviços, controladores, repositórios, gateways, adaptadores e demais elementos que compõem a lógica de negócio e suportam as funcionalidades principais.

Esse nível de modelagem permite compreender a organização interna de cada container, revelando como as responsabilidades estão distribuídas, como os módulos se relacionam e como o sistema mantém a coesão e a separação de responsabilidades. Essa visão é essencial para a manutenção, escalabilidade e evolução da arquitetura.

Abaixo, está o diagrama de componentes com os principais blocos internos organizados de acordo com suas funcionalidades.

<p align="center">
  <img src="https://drive.google.com/uc?export=view&id=1sNqbZuXpFLnevztnnJLAu596jqoP2Ohd" />
</p>

---

## Visão Geral

O sistema LIVIA.us é composto por dois containers principais:

- **Aplicativo Móvel Thunkable**
- **Backend Firebase**

Cada container possui múltiplos componentes internos, implementados como telas, módulos, lógicas de bloco ou serviços backend, conforme o caso.

---

## Aplicativo Móvel Thunkable [Container]

### Gerenciador de UI e Navegação
- Controla a lógica de navegação e qual tela será exibida ao usuário com base em seu tipo de perfil.
- Gerencia transições entre telas e inicialização do aplicativo.

### Módulo de Acessibilidade
- Integra o aplicativo com recursos do sistema operacional para garantir acessibilidade.
- Ativa leitura de tela e comandos por voz.

### Tela de Feed de Notícias
- Exibe postagens, campanhas e eventos.
- Para enfermeiros, inclui botões e formulários para criar ou editar conteúdos.

### Tela de Mapa e Geolocalização
- Mostra o mapa da cidade e as UBSs mais próximas.
- Utiliza o GPS do dispositivo e a API do Google Maps para localização e renderização visual.

### Módulo de Autenticação (UI)
- Coleta as credenciais do usuário (login/senha).
- Interface de recuperação de senha e cadastro de novos usuários.

---

## Backend Firebase [Container]

### Firebase Auth [Componente de Autenticação]
- Gerencia identidade de usuários, autenticação e recuperação de senha.

### Cloud Functions [Componente de Backend]
- Implementa a lógica do sistema sem servidor (serverless).
- Processa postagens, atualizações, chamadas de APIs externas e integrações com serviços.

### Cloud Firestore [Componente de Banco de Dados]
- Armazena todas as informações estruturadas do sistema:
  - UBSs
  - Usuários
  - Postagens
  - Campanhas
  - Dados acessados pelas telas do app

---

## Sistemas Externos

- **Sistema Operacional do Dispositivo**: fornece suporte a recursos de acessibilidade.
- **Sistema de Localização (Google Maps API)**: utilizado para exibir a posição das UBSs no mapa.
- **Sistema de E-mail**: acionado para enviar links de redefinição de senha.
- **Gov APIs**: fornece dados públicos oficiais sobre as UBSs.

---

## Conclusão

O diagrama de componentes apresenta uma arquitetura modular, em que os elementos da interface do usuário, autenticação, lógica de negócio e armazenamento de dados estão organizados de forma coesa e alinhada com boas práticas de separação de responsabilidades.

Essa visão facilita a compreensão técnica do sistema para fins de desenvolvimento, manutenção e integração com serviços externos.
