# Diagrama de Código (UML de Classes)

O diagrama de código representa a estrutura interna do sistema por meio de classes, atributos, métodos e seus relacionamentos. Este nível de detalhamento é essencial para a implementação orientada a objetos, garantindo coesão, reutilização e aderência às regras de negócio.

Por meio do diagrama de classes UML, é possível visualizar quem são os agentes principais do sistema (usuários), quais entidades compõem o domínio (UBS, Localização, Publicações) e como elas interagem entre si através de herança, associação e agregação.

<p align="center">
  <img src="https://drive.google.com/uc?export=view&id=1BA9Z_tZERhyKACZFDWt06o4erD0Btnt-" /> 
</p>

---

## Visão Geral

O sistema é modelado a partir de classes com responsabilidades específicas e bem definidas. Os principais agrupamentos de funcionalidades envolvem:

- Gestão de usuários e autenticação
- Consulta e exibição de UBSs
- Criação e edição de publicações
- Geolocalização e acessibilidade

As relações entre classes respeitam os princípios SOLID, promovendo baixo acoplamento e alta coesão.

---

## Principais Classes

### `Usuario` *(classe abstrata base)*
- Representa o modelo genérico de usuário do sistema.
- Contém atributos comuns (`id`, `nome`, `email`) e métodos como cadastro, login e recuperação de senha.
- Serve de base para as classes especializadas `UsuarioCadastrado` e `Enfermeiro`.

### `UsuarioCadastrado` *(subclasse de Usuario)*
- Representa o cidadão comum que acessa o app.
- Métodos: visualizar feed, buscar UBSs, usar o mapa, verificar acessibilidade ou perfil visitante.

### `Enfermeiro` *(subclasse de Usuario)*
- Usuário com privilégios de edição e publicação de conteúdos informativos.
- Possui `registroProfissional` e funcionalidades de CRUD sobre postagens.

### `Publicacao`
- Contém informações de postagens (título, descrição, data, autor e localização).
- Está associada a um `Enfermeiro` e a uma ou mais UBSs por meio de `localizacaoNoticia`.

### `UBS`
- Modela as Unidades Básicas de Saúde.
- Atributos: nome, horário de funcionamento, serviços oferecidos, localização e contato.
- Métodos: retornar detalhes da unidade.

### `Localizacao`
- Componente usado pela classe `UBS` para armazenar rua, bairro, número e CEP.
- Método auxiliar para retornar a string formatada da geolocalização.

### `ServicoLocalizacao`
- Responsável por integrar e abstrair chamadas à API de geolocalização do sistema externo (ex: Google Maps).
- Método: `obterGeolocalizacao()`.

### `Servicos`
- Representa os serviços oferecidos por uma UBS.
- Utilizada como composição dentro de `UBS` (relacionamento 1..*).

### `Autenticacao`
- Fornece métodos relacionados ao processo de login, cadastro e recuperação de senha.
- Trabalha em conjunto com `Usuario`.

---

## Relacionamentos Destacados

- **Herança**: `UsuarioCadastrado` e `Enfermeiro` herdam de `Usuario`, aproveitando atributos e comportamentos comuns.
- **Associação bidirecional**: Entre `Enfermeiro` e `Publicacao`, modelando o vínculo de autoria.
- **Composição**: `UBS` contém `Localizacao` e uma lista de `Servicos`.
- **Dependência**: `ServicoLocalizacao` atua como helper externo da classe `UBS`/`UsuarioCadastrado`.

---

## Conclusão

O diagrama de código oferece uma representação clara da estrutura orientada a objetos do sistema. Ele garante uma divisão lógica coerente entre agentes, serviços e entidades do domínio, facilitando a leitura, desenvolvimento colaborativo e manutenção do projeto.

Essa visão detalhada reforça o alinhamento entre a modelagem arquitetural e a codificação prática, permitindo uma evolução segura e escalável do sistema.
