# Diagrama de Containers

O diagrama de containers descreve os principais blocos de execução do sistema, como aplicações frontend, backend, bancos de dados e serviços externos. Ele mostra como esses containers se comunicam, quais são suas responsabilidades e as tecnologias utilizadas.

Esse nível de abstração é fundamental para compreender a estrutura lógica do sistema, seus fluxos de dados, e para embasar decisões relacionadas a deploy, escalabilidade e manutenção evolutiva.

A seguir, a estrutura do sistema LIVIA.us representada por containers, com destaque para seus componentes internos, serviços externos e os principais pontos de integração.

<p align="center">
  <img src="https://drive.google.com/uc?export=view&id=1cq2Z3KdReELU0A4gSHFB_usqBuWFu8DX" />
</p>

---

## Visão Geral do Sistema

### LIVIA.us [Software System]

Aplicativo móvel que permite a visualização da localização de UBSs (Unidades Básicas de Saúde), acesso a informações via mapa e feed, e interação com conteúdo publicado por enfermeiros. Implementado sobre a plataforma Thunkable, o sistema adota uma arquitetura modular, baseada em containers especializados.

---

## Containers Internos

### Aplicativo Mobile [Container: Thunkable]
- Interface utilizada por todos os perfis de usuários (visitante, cadastrado, enfermeiro, acessibilidade).
- Permite:
  - Acesso à localização de UBSs;
  - Visualização de postagens;
  - Login e recuperação de senha.

### Firebase Auth [Container: Autenticação]
- Gerencia:
  - Login com e-mail;
  - Recuperação de senha;
- Integração direta com o app móvel.

### Cloud Functions [Container: Backend]
- Executa a lógica de negócios do sistema:
  - Processamento de postagens;
  - Integrações com serviços externos;
  - Gerenciamento de conteúdo e autenticação.

### Cloud Firestore [Container: Banco de Dados]
- Armazena dados estruturados:
  - Informações de UBSs;
  - Perfis de usuários;
  - Campanhas de saúde;
  - Postagens no feed.

### Serviço de E-mail [Container: Firebase]
- Responsável por enviar e-mails automáticos para redefinição de senha.

---

## Sistemas Externos Integrados

### Sistema de Localização [Software System]
- API do Google Maps utilizada para:
  - Determinar a localização do usuário;
  - Exibir UBSs próximas no mapa.

### Gov APIs (Dados Públicos) [Software System]
- Fornece dados oficiais das UBSs e serviços públicos.
- Consultado por meio do backend do sistema.

---

## Interações entre Containers

- O aplicativo mobile usa diretamente os containers de autenticação (Firebase Auth) e backend (Cloud Functions).
- O Cloud Functions atua como núcleo de integração e processamento, consultando:
  - O banco de dados (Cloud Firestore);
  - As APIs públicas (Gov APIs);
- A recuperação de senha depende da comunicação entre o Firebase Auth e o Serviço de E-mail.
- O sistema de localização (Google Maps) é acessado diretamente pela interface do app.

---

## Conclusão

A arquitetura em containers do sistema **LIVIA.us** apresenta uma divisão de responsabilidades entre interface, lógica de negócios, persistência e serviços externos. Essa estrutura modular facilita:

- O desenvolvimento desacoplado;
- A escalabilidade de cada serviço conforme a demanda;
- A manutenção contínua de forma segura e eficiente.

