## 🔗 Rastreabilidade com Histórias do Usuário

A rastreabilidade entre as histórias do usuário e a arquitetura do sistema é uma etapa fundamental para garantir que as decisões de projeto estejam alinhadas com os requisitos funcionais levantados no início do desenvolvimento.

Nesta etapa, cada história de usuário desenvolvida no TP1 foi mapeada para os respectivos componentes do sistema que a implementam, permitindo visualizar de forma clara onde e como essas histórias se materializam na arquitetura. Além disso, foi indicado em quais diagramas arquiteturais (como os de containers, componentes ou classes) essas implementações podem ser visualizadas.

Essa abordagem favorece a manutenção, evolução e validação do sistema, uma vez que permite rastrear requisitos até sua implementação e representação arquitetural. Isso também ajuda a garantir que nenhuma funcionalidade relevante tenha sido ignorada durante o desenho da solução.

A tabela a seguir consolida essas informações:

| História do Usuário                                             | Componentes envolvidos                                   | Diagramas de referência            |
|------------------------------------------------------------------|----------------------------------------------------------|------------------------------------|
|H1 - Como usuário, eu gostaria de me cadastrar no aplicativo com email, para que eu possa fazer login e acessar as funcionalidades no app.|Thunkable , Firebase Auth , Cloud Firestore , Cloud Functions (Firebase)  | Diagramas de Containers, Componentes, Classes|
|H2 - Como usuário cadastrado, eu gostaria de fazer login com meu e-mail e senha, para que eu possa acessar as funcionalidades do app.  | DoctorDashboard, ConsultationRepository                  | Componentes, Código (classes)      |
|H3 - Como usuário cadastrado, eu gostaria de redefinir a minha senha caso eu a esqueça, para que eu possa acessar a minha conta novamente. |              xxx                                            |            xxxxxxxxxxxx                         |
| H4 - Como enfermeiro, eu gostaria de fazer login com meu e-mail, ou COREN, e senha, para que eu possa acessar as funcionalidades do app.|    xxxxxxxx  |            xxx           |
|H5 - Como visitante, eu gostaria de acessar as funcionalidades do app sem realizar cadastro, para que eu não perca tempo compartilhando meus dados.|xxxxxxxxxxxx|xxxxxxxxxxxX|
|H6 - Como usuário cadastrado/visitante, eu gostaria de ver um mapa com a localização de todas as UBSs, para que eu possa encontrar a mais próxima.|xxxxxxxxx|xxxxxxxxxx|
|H7 - Como usuário cadastrado/visitante, eu gostaria de acessar informações completas de uma UBS, para que eu saiba quais serviços ela oferece e suas áreas de atendimento.|xxxxxxx|xxxxxxX
|H8 - Como usuário cadastrado, eu gostaria de acessar facilmente todas as telas do app por um menu inferior, para que eu possa navegar rapidamente. |xxxxxxxxxxx|xxxxxxxxxxxxxxxxx|
|H9 - Como enfermeiro, eu gostaria de me cadastrar no aplicativo com email, COREN e senha, para que eu possa fazer login e acessar as funcionalidades no app.|xxxxxxxxxxxxxxx|xxxxxxxxxxx|
|H10 - Como enfermeiro, eu gostaria de poder adicionar posts, para que as pessoas possam se informar e participar das ações promovidas pela UBS, como campanhas de vacinação, seminários e entre outros.|xxxxx|Xxxxxxxxxxxx|
|H11 - Como usuário cadastrado/enfermeiro, eu gostaria de visualizar um feed com posts das UBSs, para que eu possa ficar informado sobre avisos, eventos, comunicados e entre outros.|xxxx|xxxxxx|
|H12 - Como acessibilidade, eu gostaria de navegar por todo o aplicativo usando apenas comandos de voz, para não depender do toque na tela e conseguir usar o app de forma totalmente autônoma.|xxxxxxxx|xxxxxxx|
