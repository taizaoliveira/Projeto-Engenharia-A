# Tela 1 – Cadastro de Usuário

## História de Usuário
**H1** – “Como usuário, eu gostaria de me cadastrar no aplicativo com e-mail, para que eu possa fazer login e acessar as funcionalidades no app.”

## Implementação no MVP
Tela de **Cadastro de Usuário** com formulário contendo **nome completo**, **e-mail**, **senha** e **confirmação de senha**, incluindo:

- Validação de formato de e-mail usando **regex padrão especificado**.
- Verificação de senha com mínimo de **8 caracteres**, pelo menos uma letra maiúscula e uma letra minúscula e um número.
- Checagem de campos obrigatórios e mensagens de erro em caso de preenchimento incorreto.
- Opção de marcar **acessibilidade** para usuários com deficiência.
- Verificação de **e-mail duplicado**, com redirecionamento para login caso já exista.
- Mensagem de sucesso ao finalizar, com botão para voltar para tela de login.
- Armazenamento dos dados no **Firebase Auth** e **Cloud Firestore**.

## Funcionalidade
**Cadastro de Usuário**

## Diagrama de Classes
Utiliza as classes **Usuario**, **UsuarioCadastrado**, **Autenticacao**.  
O atributo `ehAcessibilidade` é configurado na classe **UsuarioCadastrado** para marcar usuários com necessidades especiais.

## Diagrama C4 (Container)
A funcionalidade faz parte do container **“Firebase Auth”** (para autenticação) e **“Cloud Firestore”** (para armazenar dados de perfil).  
É acessada pelo container **“Aplicativo Mobile (Thunkable)”**, com interação direta com o **Serviço de E-mail** em caso de redefinição de senha.
