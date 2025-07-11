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

## Diagrama C4

- **Diagrama de Contexto:** Mostra o ator **Usuário** interagindo com o sistema **LIVIA.us**, que se comunica com o **Firebase Auth** para autenticação e o **Cloud Firestore** para armazenar dados do perfil. O fluxo também envolve o **Sistema Operacional do Dispositivo**, caso o usuário marque a opção de acessibilidade.
  
- **Diagrama de Containers:** A funcionalidade está no container **“Aplicativo Mobile (Thunkable)”**, que envia os dados de cadastro para o container **“Firebase Auth”** (autenticação) e o container **“Cloud Firestore”** (banco de dados). Caso seja necessário, aciona o **Serviço de E-mail** para fluxos de recuperação de senha.

- **Diagrama de Componentes:** Implementada pelo **Módulo de Autenticação (UI)**, que recebe os dados do formulário, faz as validações básicas e interage com o backend. O **Gerenciador de UI & Navegação** garante o redirecionamento para a tela de login após o cadastro bem-sucedido.

