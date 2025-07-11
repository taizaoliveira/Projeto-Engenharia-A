# Tela 6 – Informações Detalhadas da UBS

## História de Usuário
**H7** – “Como usuário cadastrado/visitante, eu gostaria de acessar informações completas de uma UBS, para que eu saiba quais serviços ela oferece e suas áreas de atendimento.”

## Critérios de Aceitação
- Deve ser exibida uma **imagem atualizada da fachada** da UBS.
- Devem ser exibidas as informações: **Nome Oficial**, **Endereço Completo**, **Horário de Funcionamento**, **Principais Serviços Oferecidos** e **Áreas de Atendimento**.
- A lista de **principais serviços** deve mostrar opções como: Clínica Médica, Odontologia, Vacinação, Coleta de Exames, Farmácia Popular.
- O endereço da UBS deve aparecer no formato: `"Rua, número - bairro, cidade - UF, CEP"`.
- O horário de funcionamento deve aparecer no formato: `"SEG-SEX (HH:MM-HH:MM) / SAB (HH:MM-HH:MM)"` conforme o cadastro oficial.
- O campo **"Áreas de Atendimento"** deve listar todos os bairros designados para aquela UBS.
- Deve haver um botão **"Voltar"** para retornar à tela anterior (mapa ou lista de UBSs).

## Implementação no MVP
Tela implementada no **Thunkable**, conectada ao **Cloud Firestore**, de onde são carregadas as informações detalhadas da UBS: imagem da fachada, endereço validado, horários e lista de serviços. As **Áreas de Atendimento** são exibidas de acordo com o registro oficial no banco de dados. O botão **"Voltar"** permite ao usuário retornar para o **Mapa de UBSs** ou a lista filtrada.

## Funcionalidade
**Consulta Detalhada da UBS**

## Diagrama de Classes
Utiliza as classes **UBS**, **Localizacao**, **Servicos** e **Usuario** (Cadastrado ou Visitante). A classe **Localizacao** formata o endereço conforme as regras definidas, enquanto **UBS** agrega os atributos de imagem, horário, serviços e áreas de cobertura.

## Diagrama C4

- **Diagrama de Contexto:** Mostra o ator **Usuário Cadastrado ou Visitante** interagindo com o **LIVIA.us**, que consulta o **Cloud Firestore** para carregar os dados completos de uma UBS específica. A visualização é de leitura, sem alteração de dados.

- **Diagrama de Containers:** Executado no container **“Aplicativo Mobile (Thunkable)”**, que acessa o **Cloud Firestore** para obter informações da UBS, sem necessidade de autenticação adicional para visitantes.

- **Diagrama de Componentes:** Implementado pelo **Módulo de Exibição de UBS**, responsável por renderizar imagem, endereço formatado, lista de serviços, horários e bairros atendidos. O **Gerenciador de UI & Navegação** garante o retorno à tela anterior via botão **"Voltar"**.
