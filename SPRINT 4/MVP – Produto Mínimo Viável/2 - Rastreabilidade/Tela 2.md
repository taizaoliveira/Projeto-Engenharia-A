# Tela 2 – Menu de Navegação Inferior

## História de Usuário
**H8** – “Como usuário cadastrado, quero encontrar e acessar as principais funcionalidades do aplicativo através de um menu fixo na parte inferior da tela, para que eu possa alternar entre as seções do app com clareza visual e sem atrasos na navegação.”

## Critérios de Aceitação
- Deve conter ícones intuitivos para cada funcionalidade.
- O item da tela ativa deve ter destaque visual.
- Transição suave de no máximo **0.5 segundos** entre telas.
- Ordem obrigatória do menu: **Feed**, **UBS**, **Chat**, **Perfil**.

## Implementação no MVP
Implementado como um **menu fixo (tab bar)** na parte inferior do aplicativo, utilizando os recursos do **Thunkable**. Cada ícone leva a uma tela principal: **Feed de Informações**, **Mapa das UBSs**, **Chat** e **Perfil do Usuário**. O item ativo é destacado para facilitar a usabilidade. A navegação entre telas é controlada pelo **Gerenciador de UI & Navegação**, garantindo transições suaves e tempo de resposta conforme especificado.

## Funcionalidade
**Navegação entre Telas**

## Diagrama de Classes
Relaciona-se com a classe **UsuarioCadastrado**, que acessa as funcionalidades disponíveis. A navegação é controlada pelo **Gerenciador de UI**, não sendo modelado como classe individual, mas como fluxo dentro da lógica de blocos.

## Diagrama C4 (Container)
A funcionalidade faz parte do container **“Aplicativo Mobile (Thunkable)”**, utilizando o componente **Gerenciador de UI & Navegação** que conecta as telas **Feed**, **UBS**, **Chat** e **Perfil**. Garante coesão entre front-end, backend (Firebase) e serviços externos conforme necessário.
