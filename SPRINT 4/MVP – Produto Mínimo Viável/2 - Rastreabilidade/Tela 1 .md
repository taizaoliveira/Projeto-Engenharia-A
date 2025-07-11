# Tela 1 – Cadastro de Usuário

## História de Usuário
**H1** – “Como usuário, eu gostaria de me cadastrar no aplicativo com e-mail, para que eu possa fazer login e acessar as funcionalidades no app.”

## Implementação no MVP
Tela de **Cadastro de Usuário** com formulário contendo **nome completo**, **e-mail**, **senha** e **confirmação de senha**, incluindo:

- Validação do formato de e-mail realizada com uma parte do regex padrão, utilizando apenas a verificação da presença de `'@'` e `'.'`, devido às limitações da plataforma e à complexidade do regex completo para e-mails."
- Verificação de senha com mínimo de **8 caracteres**, pelo menos uma letra maiúscula e uma letra minúscula e um número.
- Checagem de campos obrigatórios e mensagens de erro em caso de campos vazios.
- Mensagens de erro foram implementadas para os seguintes casos: e-mail em formato inválido, senha com menos de 8 caracteres, senha que não atende ao padrão esperado pelo regex, e divergência entre a senha e sua confirmação.
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
