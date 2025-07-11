# Tela 4 – Recuperação de Senha

## História de Usuário
**H3** – “Como usuário cadastrado/enfermeiro, eu gostaria de redefinir a minha senha caso eu a esqueça, para que eu possa acessar a minha conta novamente.”

## Critérios de Aceitação
- Ao clicar em **“Esqueci minha senha”** na tela de login, o usuário é direcionado para uma tela para informar o e-mail cadastrado.
- Deve existir um botão **“Voltar”** para retornar à tela de login.
- O usuário informa o e-mail para receber um link de redefinição de senha.
- Mensagem de erro se o campo de e-mail estiver vazio.
- Validações:
  1. **Formato inválido**: exibir `"Formato de e-mail inválido. Verifique e tente novamente."`
  2. **E-mail não cadastrado**: exibir `"E-mail não encontrado. Verifique se está digitado corretamente ou cadastre uma nova conta."`
- Se o e-mail for válido, enviar link seguro de redefinição para o endereço informado.
- Exibir mensagem de confirmação: `"Caso o e-mail exista, enviaremos um link para redefinição."`
- O formulário de redefinição deve conter **“Nova senha”** e **“Confirmar nova senha”**.
- A senha deve ter no mínimo **8 caracteres**, com pelo menos uma letra (maiúscula ou minúscula) e um número (`[a-z][A-Z][0-9]`).
- Mensagem de validação deve ser exibida abaixo do campo de senha indicando se os requisitos foram atendidos.
- O link de redefinição expira em **1 hora** e só pode ser usado uma vez.
- Se o link for inválido ou expirado, deve-se exibir: `"Este link de redefinição é inválido ou expirou. Por favor, solicite um novo link."`

## Implementação no MVP
Fluxo de recuperação de senha implementado no **Thunkable**, integrado ao **Firebase Auth** e ao **Serviço de E-mail** do Firebase. O usuário informa o e-mail, que é validado com regex e verificado no banco. Em caso de sucesso, um link de redefinição seguro é enviado. O formulário de redefinição de senha aplica as validações de segurança e o link expira conforme a regra de negócio. Mensagens de erro e sucesso são exibidas em todos os pontos necessários.

## Funcionalidade
**Recuperação de Senha**

## Diagrama de Classes
Utiliza as classes **Usuario**, **Autenticacao**.

## Diagrama C4 

- **Diagrama de Contexto:** Mostra os atores **Usuário Cadastrado** ou **Enfermeiro** interagindo com o sistema **LIVIA.us**, que se conecta ao **Firebase Auth** para verificar o e-mail, gerar o link de redefinição e também aciona o **Serviço de E-mail** para enviar o link seguro ao usuário.

- **Diagrama de Containers:** A funcionalidade é executada no container **“Aplicativo Mobile (Thunkable)”**, que se comunica com o container **“Firebase Auth”** (gerenciamento da redefinição de senha) e o **Serviço de E-mail** (envio do link). O **Cloud Firestore** é usado para armazenar informações relacionadas ao usuário.

- **Diagrama de Componentes:** Implementada pelo **Módulo de Autenticação (UI)**, responsável por coletar o e-mail, validar o formato, exibir mensagens de erro e sucesso e renderizar o formulário de nova senha. O **Gerenciador de UI & Navegação** gerencia o fluxo entre telas (login ↔ recuperação) e o redirecionamento após o reset.
