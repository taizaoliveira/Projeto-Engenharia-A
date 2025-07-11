# Tela 3 – Login

## História de Usuário
**H2** – “Como usuário cadastrado, eu gostaria de fazer login com meu e-mail e senha, para que eu possa acessar as funcionalidades do app.”

## Critérios de Aceitação
- O usuário deve informar **e-mail** e **senha**.
- Botão **“Entrar”** para enviar as credenciais.
- Exibir mensagem de erro **“E-mail ou senha inválidos.”** caso as credenciais estejam incorretas.
- Exibir mensagem de erro **“Por favor, preencha todos os campos.”** caso estejam vazios.
- Ícone para mostrar/ocultar a senha digitada.
- Botão **“Cadastrar”** para iniciar o fluxo de cadastro.
- Sensível a maiúsculas/minúsculas: o login e a senha devem ser digitados exatamente como cadastrados.
- Link recuperação de senha.

## Implementação no MVP
Tela de **Login** com formulário de entrada de **e-mail** e **senha**, incluindo opção para mostrar/ocultar a senha digitada. Após clicar em **“Entrar”**, o sistema verifica as credenciais no **Firebase Auth**. Se inválidas ou vazias, exibe mensagens de erro específicas. O botão **“Cadastrar”** redireciona para o fluxo de cadastro. Existe link **“Esqueci minha senha”** para recuperação. Todas as validações de autenticação são sensíveis a letras maiúsculas/minúsculas, como definido nos critérios.

## Funcionalidade
**Autenticação de Usuário**

## Diagrama de Classes
Utiliza as classes **Usuario**, **Autenticacao**.

## Diagrama C4 (Container)
A funcionalidade faz parte do container **“Firebase Auth”** (autenticação) e é acessada pelo container **“Aplicativo Mobile (Thunkable)”**. Interage com o **Serviço de E-mail** em caso de recuperação de senha.
