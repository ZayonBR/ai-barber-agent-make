# ai-barber-agent-make
Automação de agendamento via WhatsApp utilizando Make, Google Gemini e Google Calendar.

# 💈 AI Barber Agent - Automação com Make, Webhooks e IA

Este projeto demonstra a construção de um Agente de Agendamento Automatizado utilizando a plataforma **Make**. O sistema orquestra múltiplas APIs para simular um atendimento humano no WhatsApp.

![Fluxo do Projeto](fluxo-completo.png)

## 🛠️ Arquitetura e Aprendizados

O projeto foi desenvolvido em **Low-Code**, mas fundamentado em conceitos sólidos de integração de sistemas:

* **Make (Integromat):** Utilizado como orquestrador do back-end.
* **Webhooks:** Implementados para escutar eventos de entrada (mensagens do WhatsApp) em tempo real, garantindo resposta imediata.
* **Integração de APIs:**
    * **Z-API:** Gateway para envio e recebimento de mensagens do WhatsApp.
    * **Google Gemini (AI):** Processamento de Linguagem Natural (NLP) via API para interpretar a intenção do usuário e extrair datas.
    * **Google Calendar API:** Manipulação de eventos (CRUD) para verificar disponibilidade e criar agendamentos.
* **Manipulação de JSON:** Estruturação de payloads para comunicação entre os módulos e a IA.

## 🚀 Funcionalidades

1.  **Webhook Trigger:** Recebimento de mensagem instantânea.
2.  **State Management:** Consulta de histórico em Data Store (Memória persistente).
3.  **AI Decision Making:** O Gemini decide se deve responder uma dúvida ou agendar um horário.
4.  **API Action:** Agendamento automático na agenda (Google Calendar).

## 📦 Como testar

O arquivo `blueprint.json` deste repositório contém toda a lógica do cenário.
1. Baixe o arquivo.
2. No Make, crie um novo cenário.
3. Clique em `More` (...) -> `Import Blueprint`.

---
*Desenvolvido com foco em automação e integração de sistemas.*
