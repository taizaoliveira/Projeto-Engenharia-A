
# Diagrama de Contexto

O diagrama de contexto representa o sistema como uma "caixa preta", destacando os atores externos (usuários e sistemas) que interagem com ele e os fluxos principais de comunicação. Essa visão facilita a compreensão das fronteiras do sistema, revelando suas interfaces com agentes humanos e outros sistemas que o apoiam ou dependem de suas funcionalidades.   

Abaixo, são apresentados os principais perfis envolvidos e os sistemas com os quais o sistema central se comunica para cumprir suas funções essenciais.


<p align="center">
  <img src="https://drive.google.com/uc?export=view&id=1feFrN6bRSbWmYNtI5quB8IsZD79EUzaL" />
</p>

## Visão Geral – Aplicativo LIVIA.us

O diagrama representa, em alto nível, o funcionamento do sistema **LIVIA.us**, um aplicativo voltado à visualização de informações e acesso às Unidades Básicas de Saúde (UBSs) do município de Itacoatiara (AM). Ele apresenta os principais atores humanos e sistemas externos que interagem diretamente com o sistema central.

---

## Sistema Central

### **LIVIA.us [Software System]**
Aplicativo de localização e acesso à informação sobre UBSs. Atua como o núcleo do sistema, integrando usuários e serviços externos como autenticação, localização e dados públicos.

---

## Atores do Sistema (Pessoas)

- **Usuário Cadastrado**  
  Cidadão com conta ativa. Realiza login, acessa o feed e consulta UBSs.

- **Visitante**  
  Pessoa que acessa o app sem login. Navega livremente para consultar informações básicas sobre UBSs.

- **Enfermeiro**  
  Profissional de saúde responsável por atualizar e manter as informações do sistema.

- **Pessoa com Acessibilidade**  
  Usuário com deficiência (visual ou motora), que interage com o sistema utilizando recursos assistivos como leitura de tela e comandos de voz.

---

## 🔗 Sistemas Externos Integrados

- **Firebase (Backend)**  
  Backend do aplicativo. Gerencia:
  - Autenticação
  - Armazenamento de dados
  - Recuperação de informações

- **Sistema de E-mail**  
  Responsável por envio de e-mails de recuperação de senha.

- **Sistema de Localização (Google Maps API)**  
  Fornece localização das UBSs. Permite ao usuário localizar unidades próximas.

- **Gov APIs (Dados Públicos)**  
  Integração com API do governo para obter dados oficiais sobre UBSs.

- **Sistema Operacional do Dispositivo**  
  Suporta recursos de acessibilidade (como leitura de tela e comandos por voz), adaptando o app às necessidades do usuário.

---

## Interações-Chave

- **Usuário cadastrado**: realiza login e consulta dados via LIVIA.us.
- **Visitante**: acessa informações básicas sem autenticação.
- **Enfermeiro**: atualiza dados do sistema.
- **Pessoa com acessibilidade**: utiliza o app com suporte do sistema operacional.
- **LIVIA.us**:
  - Integra-se com o Firebase para autenticação e dados.
  - Consulta o sistema de e-mail para recuperação de senha.
  - Usa a Google Maps API para localização.
  - Obtém dados oficiais via Gov APIs.

---

## Conclusão

O diagrama demonstra um ecossistema tecnológico acessível e integrado, centrado no usuário. O **LIVIA.us** conecta cidadãos e profissionais à rede pública de saúde por meio de:
- tecnologias modernas (Firebase, APIs do governo),
- suporte à acessibilidade,
- e acesso geolocalizado às UBSs.

