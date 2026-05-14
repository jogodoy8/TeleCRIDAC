# TeleCRIDAC - Plataforma de Teleatendimento Multidisciplinar CRIDAC/SES-MT

## 📋 Visão Geral
O **TeleCRIDAC** é uma plataforma de telessaúde customizada para o **Centro de Reabilitação Dom Aquino Corrêa (CRIDAC)**. O projeto visa viabilizar o atendimento remoto multidisciplinar (Fisioterapia, Fonoaudiologia, Psicologia, entre outros) de forma resiliente, segura e gratuita.

[cite_start]A arquitetura segue a **Tática do "Aparentemente Simples"**: complexidade robusta no back-end para garantir a integridade dos dados, com uma interface de extrema simplicidade no front-end para o cidadão[cite: 1, 7].

## 🚀 Fluxo de Atendimento
O sistema operacionaliza as etapas fundamentais do cuidado remoto:

1.  [cite_start]**Agendamento e Notificação:** Integração com a base de dados de regulação e disparo automático de link único via SMS/WhatsApp 15 minutos antes da consulta[cite: 1, 10, 11].
2.  [cite_start]**Check-in e Sala de Espera:** Página de teste automático de câmera e microfone com status em tempo real para o paciente[cite: 1, 12, 14].
3.  [cite_start]**Teleconsulta (Videochamada):** Uso de tecnologia WebRTC para atendimento em tempo real sem plugins, com painel dividido para preenchimento do formulário **IFBrM** pelo especialista[cite: 1, 16, 19, 20].
4.  [cite_start]**Finalização e Auditoria:** Registro automático de duração para faturamento SUS e gatilho de pesquisa de satisfação[cite: 2, 30, 31].

## 🛠️ Pilares Tecnológicos (Foco em Gratuidade e Robustez)
Desenvolvido com ferramentas open-source e camadas gratuitas (tiers) para garantir custo zero de implementação:

* **Comunicação:** Jitsi Meet SDK (WebRTC).
* **Banco de Dados e Logs:** Supabase (PostgreSQL).
* **Automação de Mensagens:** Make.com / Evolution API.
* **Dashboards de Gestão:** Google Looker Studio / Metabase.

## 🔒 Segurança e LGPD
Em conformidade com a Lei Geral de Proteção de Dados:
* [cite_start]**Criptografia:** Comunicação protegida de ponta a ponta[cite: 2, 33].
* [cite_start]**Privacidade:** Nenhuma gravação de imagem ou áudio sem consentimento clínico explícito[cite: 2, 33].
* [cite_start]**Resiliência:** Implementação de monitoramento ativo e botão de reconexão rápida para instabilidades de banda[cite: 2, 35, 36].

## ♿ Acessibilidade
[cite_start]Interface desenhada especificamente para pessoas com deficiência, garantindo compatibilidade com leitores de tela e alto contraste[cite: 2, 37].

## 📈 Inteligência de Dados (CGA)
A plataforma gera logs interoperáveis (JSON/CSV) para monitoramento de KPIs pela Coordenação de Gestão Ambulatorial:
* [cite_start]Taxa de latência média e sucesso de conexão[cite: 2, 39, 40, 41].
* Produtividade por profissional e especialidade.
* [cite_start]Alcance territorial via geolocalização do acesso[cite: 2, 42].

---
**Desenvolvido por:** Joelma Godoy
**Instituição:** Secretaria Estadual de Saúde de Mato Grosso (SES/MT) / CRIDAC
