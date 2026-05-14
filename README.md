# TeleCRIDAC - Plataforma de Teleatendimento Multidisciplinar CRIDAC/SES-MT

## 📋 Visão Geral
O **TeleCRIDAC** é uma plataforma de telessaúde customizada para o **Centro de Reabilitação Dom Aquino Corrêa (CRIDAC)**. O projeto visa viabilizar o atendimento remoto multidisciplinar (Fisioterapia, Fonoaudiologia, Psicologia, entre outros) de forma resiliente, segura e gratuita.

A arquitetura segue a **Tática do "Aparentemente Simples"**: complexidade robusta no back-end para garantir a integridade dos dados, com uma interface de extrema simplicidade no front-end para o cidadão.

## 🚀 Fluxo de Atendimento
O sistema operacionaliza as etapas fundamentais do cuidado remoto:

1. **Agendamento e Notificação:** Integração com a base de dados de regulação e disparo automático de link único via SMS/WhatsApp 15 minutos antes da consulta.
2.  **Check-in e Sala de Espera:** Página de teste automático de câmera e microfone com status em tempo real para o paciente.
3.  **Teleconsulta (Videochamada):** Uso de tecnologia WebRTC para atendimento em tempo real sem plugins, com painel dividido para preenchimento do formulário **IFBrM** pelo especialista.
4.  **Finalização e Auditoria:** Registro automático de duração para faturamento SUS e gatilho de pesquisa de satisfação.

## 🛠️ Pilares Tecnológicos (Foco em Gratuidade e Robustez)
Desenvolvido com ferramentas open-source e camadas gratuitas (tiers) para garantir custo zero de implementação:

* **Comunicação:** Jitsi Meet SDK (WebRTC).
* **Banco de Dados e Logs:** Supabase (PostgreSQL).
* **Automação de Mensagens:** Make.com / Evolution API.
* **Dashboards de Gestão:** Google Looker Studio / Metabase.

## 🔒 Segurança e LGPD
Em conformidade com a Lei Geral de Proteção de Dados:
* **Criptografia:** Comunicação protegida de ponta a ponta.
* **Privacidade:** Nenhuma gravação de imagem ou áudio sem consentimento clínico explícito.
* **Resiliência:** Implementação de monitoramento ativo e botão de reconexão rápida para instabilidades de banda.

## ♿ Acessibilidade
Interface desenhada especificamente para pessoas com deficiência, garantindo compatibilidade com leitores de tela e alto contraste.

## 📈 Inteligência de Dados (CGA)
A plataforma gera logs interoperáveis (JSON/CSV) para monitoramento de KPIs pela Coordenação de Gestão Ambulatorial:
* Taxa de latência média e sucesso de conexão.
* Produtividade por profissional e especialidade.
* Alcance territorial via geolocalização do acesso.

---
**Desenvolvido por:** Joelma Silva Campos Godoy  
**Instituição:** Secretaria Estadual de Saúde de Mato Grosso (SES/MT) \ CRIDAC
