# Tela 7 – Feed de Posts das UBSs

## História de Usuário
**H11** – “Como usuário cadastrado/enfermeiro, eu gostaria de visualizar um feed com posts das UBSs, para que eu possa ficar informado sobre avisos, eventos, comunicados e entre outros.”

## Critérios de Aceitação
- Os posts devem ser exibidos em **ordem cronológica**, do mais recente para o mais antigo.
- Deve permitir **navegação por scroll**, rolando os conteúdos sem interrupção.
- Cada post deve exibir: **Título**, **Imagem**, **Data de Publicação**, **Local** e **Descrição** (se houver).

## Implementação no MVP
Tela do **Feed** implementada no **Thunkable**, conectada ao **Cloud Firestore**, onde os **posts** são salvos por data. O **Gerenciador de UI & Navegação** carrega os posts ordenados automaticamente do mais recente para o mais antigo, permitindo rolagem vertical infinita. Cada item do feed mostra título, imagem, data, local de publicação e descrição, se houver.

## Funcionalidade
**Visualização de Feed**

## Diagrama de Classes
Utiliza as classes **Publicacao**, **Enfermeiro** e **UsuarioCadastrado**. A classe **Publicacao** possui atributos como título, imagem, data, local e descrição, vinculada a um autor (**Enfermeiro**) e exibida para o **UsuarioCadastrado**.

## Diagrama C4

- **Diagrama de Contexto:** Mostra os atores **Usuário Cadastrado** e **Enfermeiro** interagindo com o **LIVIA.us**, que consulta o **Cloud Firestore** para carregar os posts atualizados no feed.

- **Diagrama de Containers:** O fluxo roda no container **“Aplicativo Mobile (Thunkable)”**, que acessa o **Cloud Firestore** para ler as publicações em tempo real. O **Firebase Auth** garante a autenticação do usuário cadastrado/enfermeiro.

- **Diagrama de Componentes:** Implementado pelo **Módulo de Feed**, que renderiza os posts ordenados com rolagem. O **Gerenciador de UI & Navegação** gerencia o scroll, a atualização dos posts e a exibição dos detalhes (título, imagem, data, local e descrição).
