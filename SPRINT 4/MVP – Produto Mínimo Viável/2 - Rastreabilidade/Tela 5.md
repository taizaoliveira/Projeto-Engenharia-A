# Tela 5 – Acesso como Visitante

## História de Usuário
**H5** – “Como visitante, eu gostaria de acessar as funcionalidades do app sem realizar cadastro, para que meus dados não precisem ser inseridos toda vez que eu acessar o aplicativo.”

## Critérios de Aceitação
- Deve existir um botão **“Entrar sem cadastro”** na tela de login.
- Assim que o visitante entrar, deve informar o **CEP** da sua cidade no formato: `"5 dígitos + hífen + 3 dígitos"`.
- O botão para prosseguir só será habilitado após digitar um CEP no formato válido e validado como existente via **API do Google Maps**.
- Se o CEP for inválido ou inexistente, o sistema deve exibir uma mensagem de erro informando que o CEP não é válido.
- O visitante não poderá prosseguir enquanto o CEP não for validado.
- Após a validação de um CEP válido, o visitante terá acesso limitado: poderá apenas visualizar a localização das UBSs no mapa e consultar áreas de cobertura.

## Implementação no MVP
Implementado no **Thunkable**, com botão **“Entrar sem cadastro”** na tela de login. O visitante é direcionado para informar o **CEP**, que é validado com regex básico (formato `XXXXX-XXX`) e verificado na **Google Maps API** para confirmar se é real. Se válido, o usuário é liberado para acessar as telas de **Mapa das UBSs** e **Cobertura Territorial** com acesso restrito (sem feed ou chat). Caso o CEP seja inválido ou inexistente, uma mensagem de erro é exibida.

## Funcionalidade
**Acesso como Visitante**

## Diagrama de Classes
Utiliza a classe **Usuario** (modo anônimo), **ServicoLocalizacao** para validar o CEP e **UBS** para exibir unidades no mapa e áreas de cobertura.

## Diagrama C4

- **Diagrama de Contexto:** Mostra o ator **Visitante** interagindo com o **LIVIA.us**, que consulta o **Google Maps API** para validação do CEP e exibição de localização das UBSs. O **Cloud Firestore** fornece dados de cobertura, mas sem registrar informações pessoais.

- **Diagrama de Containers:** O fluxo roda no container **“Aplicativo Mobile (Thunkable)”**, que se conecta ao **Sistema de Localização (Google Maps API)** para validar o CEP e renderizar o mapa com UBSs. O **Cloud Firestore** é acessado apenas para leitura de dados de unidades e áreas atendidas.

- **Diagrama de Componentes:** Implementado pelo **Gerenciador de UI & Navegação**, que controla o fluxo de entrada como visitante, coleta e valida o CEP, exibe mensagens de erro e libera o acesso restrito às telas **Mapa de UBSs** e **Cobertura Territorial**. O **Módulo de Localização** realiza a integração com a **API do Google Maps**.
