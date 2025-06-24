# Revisão da Inspeção de Requisitos

Nesta etapa do trabalho, revisamos e analisamos os apontamentos identificados como defeitos nos requisitos. Verificamos cada issue registrada, confirmamos aquelas que de fato representavam problemas e realizamos as devidas correções. Também identificamos quais apontamentos não correspondiam a defeitos, classificando-os como não confirmados ou reavaliados.

## Tabela de Defeitos

| **ISSUES**                         | **QUANTIDADE** | **LOCALIZAÇÃO**                                                                 |
|-----------------------------------|----------------|----------------------------------------------------------------------------------|
| Número de Defeitos                | 38             | #2 - #39                                                                         |
| Issues Confirmadas e Corrigidas   | 33             | #2 , #3, #5 - #12, #14 - #30, #32 - #34, #36 , #37, #39                          |
| Issues Não Confirmadas            | 4              | #4, #31, #35, #38                                                                |
| Issues Reavaliadas                | 1              | #13                                                                             |

---

##  Issues Resolvidas


###  Validações e Segurança

- **E-mail**: Regex corrigida para aceitar qualquer domínio válido e permitir caracteres especiais, com regras claras para o uso do ponto (.).
- **Senha**: Regras de complexidade definidas (mínimo uma letra maiúscula, uma minúscula e um número).
- **Login**: Comportamento de sensibilidade a maiúsculas/minúsculas (case sensitive) especificado.

###  Mensagens de Erro

- Mensagens mais claras e específicas para e-mail/senha inválidos ou campos vazios.
- Erros no fluxo de recuperação de senha agora distinguem “formato inválido” e “e-mail não encontrado”.

###  Fluuxos e Navegação

- Recuperação de senha: Fluxo completo documentado, incluindo expiração e reuso de links.
- Login de enfermeiro: Campo unificado para e-mail ou COREN com formato padronizado.
- Visitante: Validação de CEP aprimorada com API e mensagens específicas.

###  Mapa e UBS

- Integração com Google Maps definida.
- Lógica de ordenação de UBSs (por proximidade ou alfabética) formalizada.
- Exibição detalhada de UBSs: endereço, telefone, horário e serviços.

###  Acessibilidade e Clareza

- Textos vagos substituídos por descrições objetivas.
- Linguagem inclusiva aplicada em histórias com foco em acessibilidade.

###  Processos Internos

- Publicação de eventos: Fluxo de aprovação por responsáveis definido, com notificações e possibilidade de ativação/desativação no painel administrativo.

---

##  Issues Não Confirmadas

###  Telas e Menus (H1, H8)

- **Botão "Voltar para tela inicial" (H1)**:
  - Não existe essa funcionalidade nos critérios. O botão já previsto é para retornar ao login, conforme esperado.

- **Ordem do Menu (H8)**:
  - A ordem “Feed, UBS, Chat, Perfil” já estava claramente listada nos critérios, sem omissões.

###  Escopo e Contexto (H10, H11)

- **Divisão de funcionalidades (H10)**:
  - A história possui um objetivo funcional único (publicação de eventos). Não há necessidade de separação em outras histórias.

- **Comandos de voz (H11)**:
  - A história trata apenas da visualização de posts. O uso de voz está corretamente tratado na H12, e a issue estava atribuída de forma incorreta.

---

##  Issues Reavaliadas

###  Uso Único do Link de Redefinição (H3)

- Regra “link só pode ser usado uma vez” revisada.
- Classificada como regra técnica, não exigindo inclusão nos critérios de aceitação.
- Documentada nas regras de negócio com mensagem orientativa ao usuário em caso de uso ou expiração.
- Issue encerrada sem alterações nos critérios.

---

As issues revisadas nesta etapa foram originalmente identificadas e descritas no documento **“Inspeção do Backlog"**, o qual apresenta detalhadamente os critérios de aceitação, descrições dos defeitos, tipo de falha e sua classificação. Esse documento serviu como base para a verificação, categorização e tratamento das ocorrências nesta fase da inspeção, e pode ser consultado no link a seguir:

[Inspeção do Backlog (PDF)](https://github.com/taizaoliveira/Projeto-Engenharia-A/blob/main/SPRINT%203/Casos%20de%20Testes/1%20-%20%20Revis%C3%A3o%20da%20Inspe%C3%A7%C3%A3o%20de%20Requisitos/Inspe%C3%A7%C3%A3o%20do%20Backlog.pdf)

