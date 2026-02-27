
# Teste Manual – Carteira de Trabalho Digital

## 📌 Objetivo
Avaliar o fluxo de autenticação do aplicativo Carteira de Trabalho Digital, com foco na validação funcional, verificação em duas etapas (2FA) e comportamento de redirecionamento entre aplicações.

---

## 🔎 Escopo do Teste
O teste exploratório foi focado exclusivamente no fluxo de login, incluindo:

- Autenticação via gov.br (CPF e senha)
- Login via banco (mobile e desktop)
- Verificação em duas etapas (2FA)
- Redirecionamento entre aplicações
- Validação de mensagens e comportamento do sistema

Não foram testadas funcionalidades internas após login bem-sucedido.

---

## 🧪 Ambiente de Teste

- Dispositivo Mobile: Xiaomi Redmi Note 14
- Sistema Operacional Mobile: Android 15
- Ambiente Desktop: Windows 10 Pro
- Navegador: Google Chrome (64 bits)
- Aplicativo Gov.br: Versão 3.8.0
- Aplicativo Carteira de Trabalho Digital: Versão 8.6.0
- Data do teste: 27/02/2026

---

## 🚨 Principais Achados

### 1️⃣ Falha na geração de código 2FA
- O sistema solicita código de verificação, porém não permite geração ou conclusão adequada do processo.
- Severidade: Alta  
- Impacto: Impede conclusão do login.

### 2️⃣ Falha de redirecionamento (Mobile)
- Após autenticação via banco, o sistema não redireciona automaticamente para o aplicativo Carteira de Trabalho Digital.
- Severidade: Alta  
- Impacto: Interrompe fluxo de acesso.

### 3️⃣ Verificação redundante (Desktop)
- Mesmo após autenticação via banco com QR Code, o sistema solicita nova verificação por código de acesso.
- Severidade: Alta  
- Impacto: Impede acesso ao serviço.

---

## 📄 Relatório Completo

O relatório detalhado pode ser consultado no arquivo:

*Relatorio_Teste_CT_Digital_2026-02-27_v1.pdf*

---

## 🎯 Considerações

O fluxo de autenticação apresenta falhas críticas que impedem o acesso ao serviço, afetando diretamente a experiência do usuário e a confiabilidade do sistema.
