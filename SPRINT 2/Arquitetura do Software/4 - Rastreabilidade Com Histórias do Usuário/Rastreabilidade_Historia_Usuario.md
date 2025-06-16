## 🔗 Rastreabilidade com Histórias do Usuário

A rastreabilidade entre as histórias do usuário e a arquitetura do sistema é uma etapa fundamental para garantir que as decisões de projeto estejam alinhadas com os requisitos funcionais levantados no início do desenvolvimento.

Nesta etapa, cada história de usuário desenvolvida no TP1 foi mapeada para os respectivos componentes do sistema que a implementam, permitindo visualizar de forma clara onde e como essas histórias se materializam na arquitetura. Além disso, foi indicado em quais diagramas arquiteturais (como os de containers, componentes ou classes) essas implementações podem ser visualizadas.

Essa abordagem favorece a manutenção, evolução e validação do sistema, uma vez que permite rastrear requisitos até sua implementação e representação arquitetural. Isso também ajuda a garantir que nenhuma funcionalidade relevante tenha sido ignorada durante o desenho da solução.

A tabela a seguir consolida essas informações:

| História do Usuário                                             | Componentes envolvidos                                   | Diagramas de referência            |
|------------------------------------------------------------------|----------------------------------------------------------|------------------------------------|
|H1 - Como usuário, eu gostaria de me cadastrar no aplicativo com email, para que eu possa fazer login e acessar as funcionalidades no app.|Thunkable , Firebase Auth , Cloud Firestore , Cloud Functions (Firebase)  | Diagramas de Containers, Componentes, Classes|
|H2 - Como usuário cadastrado, eu gostaria de fazer login com meu e-mail e senha, para que eu possa acessar as funcionalidades do app.  | Thunkable , Firebase Auth    |Diagramas de Containers, Componentes, Classes    |
|H3 - Como usuário cadastrado, eu gostaria de redefinir a minha senha caso eu a esqueça, para que eu possa acessar a minha conta novamente. |Thunkable , Firebase Auth                       |Containers, Componentes, Fluxo de Navegação|
|H4 - Como enfermeiro, eu gostaria de fazer login com meu e-mail, ou COREN, e senha, para que eu possa acessar as funcionalidades do app.|   Thunkable , Firebase Auth , Cloud Functions (Firebase) , Cloud Firestore  |      Diagramas de Containers, Componentes, Classes   |
|H5 - Como visitante, eu gostaria de acessar as funcionalidades do app sem realizar cadastro, para que eu não perca tempo compartilhando meus dados.|Thunkable, Google Maps API, GOV APIs, Cloud Firestore | Diagramas de Containers, Componentes|
|H6 - Como usuário cadastrado/visitante, eu gostaria de ver um mapa com a localização de todas as UBSs, para que eu possa encontrar a mais próxima.|Thunkable, Cloud Functions (Firebase), Cloud Firestore, Google Maps API, GOV APIs|Diagramas de Containers, Componentes|
|H7 - Como usuário cadastrado/visitante, eu gostaria de acessar informações completas de uma UBS, para que eu saiba quais serviços ela oferece e suas áreas de atendimento.|Thunkable , GOV APIs , Cloud Firestore |Containers, Componentes, Fluxo de Navegação 
|H8 - Como usuário cadastrado, eu gostaria de acessar facilmente todas as telas do app por um menu inferior, para que eu possa navegar rapidamente. |Thunkable, Figma|Containers, Componentes, Fluxo de Navegação |
|H9 - Como enfermeiro, eu gostaria de me cadastrar no aplicativo com email, COREN e senha, para que eu possa fazer login e acessar as funcionalidades no app.|Tela de Cadastro (Thunkable); Cloud Functions ; Banco de Dados: Cloud Firestore; Autenticação: Firebase Auth |Diagrama de Containers, Diagrama de Classes, Diagrama de Componentes|
|H10 - Como enfermeiro, eu gostaria de poder adicionar posts, para que as pessoas possam se informar e participar das ações promovidas pela UBS, como campanhas de vacinação, seminários e entre outros.|Thunkable, Firebase Auth, Cloud Firestore, Cloud Functions (Firebase)|Diagramas de Containers, Componentes, Classes|
|H11 - Como usuário cadastrado/enfermeiro, eu gostaria de visualizar um feed com posts das UBSs, para que eu possa ficar informado sobre avisos, eventos, comunicados e entre outros.|Thunkable, Firebase Auth, Cloud Firestore, Cloud Functions (Firebase)|Diagramas de Containers, Componentes, Classes|
|H12 - Como acessibilidade, eu gostaria de navegar por todo o aplicativo usando apenas comandos de voz, para não depender do toque na tela e conseguir usar o app de forma totalmente autônoma.|Thunkable, APIs NativasThunkable, APIs Nativas (Acessibilidade), Figma|Diagramas de Containers, Componentes|
