Conjunto fictício de requisitos para um software de gerenciamento de eventos chamado "EventEase":

# Requisitos Funcionais e Não Funcionais - EventEase

## Requisitos Funcionais:

1. **Cadastro de Eventos:**
   - O sistema deve permitir que os organizadores cadastrem novos eventos com informações como:
     - Nome
     - Data
     - Horário
     - Local
     - Descrição
   - O organizador pode categorizar os eventos (Ex.: Conferência, Workshop, Reunião, Social).

2. **Controle de Participantes:**
   - O sistema deve permitir que os usuários se inscrevam nos eventos com informações básicas como:
     - Nome
     - E-mail
     - Telefone
   - O sistema deve gerar automaticamente um **QR Code** único para cada participante, que será utilizado para o check-in no evento.

3. **Emissão de Certificados:**
   - O sistema deve gerar certificados de participação personalizados com base no nome do participante e no evento em questão.
   - Os organizadores devem poder configurar um **template padrão** de certificado com:
     - Logotipo
     - Assinatura
     - Layout predefinido

## Requisitos Não Funcionais:

4. **Performance:**
   - O sistema deve suportar até **1.000 usuários simultâneos** sem perda significativa de desempenho.
   - O tempo de resposta para a execução de ações (cadastro, inscrição, emissão de certificado) deve ser inferior a **2 segundos**.

5. **Segurança:**
   - O sistema deve utilizar autenticação por **OAuth 2.0** para garantir a segurança dos dados dos usuários.
   - Os dados dos participantes devem ser **criptografados** no banco de dados utilizando **AES-256**.

6. **Compatibilidade:**
   - O sistema deve ser responsivo e compatível com os navegadores:
     - Google Chrome
     - Mozilla Firefox
     - Safari (nas suas três últimas versões)
   - O sistema deve oferecer suporte para dispositivos móveis (Android e iOS) com **layout adaptado**.
