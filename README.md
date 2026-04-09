# 🦈 Shark Web Monitor

Monitor de rede em tempo real focado em **impacto real nos aplicativos web**.  
Ao invés de mostrar apenas números, ele traduz latência, quedas e oscilações em **efeitos práticos para o usuário**.

---

## 🚀 Visão geral

O **Shark Web Monitor** é uma ferramenta front-end (100% client-side) que mede a latência da conexão e apresenta:

- 📡 Status da conexão em tempo real  
- ⚡ Impacto direto nos apps web (ERP, CRM, sistemas internos, etc)  
- 📊 Histórico de latência com gráfico  
- 🚨 Alertas inteligentes e explicativos  
- 🧠 Score de saúde da rede (0–100)  

---

## 🖥️ Preview

Interface moderna com:

- Banner de impacto (claro e direto)
- Cards de métricas principais
- Gráfico de latência
- Logs e alertas explicativos
- Escala visual de impacto

---

## ⚙️ Funcionalidades

### 📡 Monitoramento em tempo real
- Mede latência continuamente via `fetch`
- Alterna entre múltiplos endpoints (Google, Cloudflare, etc)

### 🧠 Interpretação inteligente
- Não mostra só ms → mostra impacto:
  - ✅ Ótimo
  - ⚠️ Atenção
  - 🟠 Lento
  - 🔴 Crítico

### 🚨 Sistema de alertas
- Detecta:
  - Quedas de conexão
  - Oscilações bruscas
  - Lentidão persistente
- Explica o que isso causa nos sistemas

### 📊 Health Score
Pontuação baseada em:
- Latência média
- Taxa de quedas
- Oscilações

### 📉 Gráfico de histórico
- Visualização em tempo real
- Destaque para eventos críticos

### 🔔 Notificações
- Toasts visuais
- Som opcional
- Notificações do navegador

### ⚙️ Configurações
- Intervalo de verificação
- Limite de lentidão
- Sensibilidade de oscilação
- Alertas sonoros

### 📁 Exportação
- CSV (logs)
- TXT (relatório)

---

## 🧩 Tecnologias usadas

- HTML5
- CSS3 (UI moderna, dark mode)
- JavaScript (Vanilla)
- Chart.js

---

## 📦 Como usar

### 1. Clone o repositório
```bash
git clone https://github.com/seu-usuario/shark-web-monitor.git

📦 Como usar
1. Clone o repositório
git clone https://github.com/seu-usuario/shark-web-monitor.git
2. Abra o arquivo

Basta abrir no navegador:

SharkWebmonitor.html

Não precisa de servidor, backend ou instalação.

Ou Pode usar Vercel : https://shark-web-monitor.vercel.app/

🧠 Como funciona

O sistema mede latência usando requisições HTTP para endpoints leves:

fetch('https://www.google.com/favicon.ico')

Depois calcula:

Tempo de resposta (ms)
Média dos últimos pings
Oscilações entre medições
Quedas (timeout)

E traduz isso para impacto real nos apps.

📊 Faixas de impacto
Latência	Impacto
< 80ms	✅ Excelente
80–200ms	👍 Bom
200–400ms	⚠️ Atenção
400–1000ms	🟠 Lento
> 1000ms	🔴 Crítico
🎯 Objetivo do projeto

A maioria das ferramentas mostra números técnicos.
Este projeto foca em:

"O que isso realmente causa no sistema que o usuário está usando?"

🔐 Limitações
Depende do navegador (CORS / bloqueios podem afetar)
Não substitui ferramentas profissionais de monitoramento
Mede latência HTTP, não ICMP (ping real)

💡 Ideias futuras
Backend para histórico persistente
Integração com APIs (Grafana, Prometheus)
Monitoramento de múltiplos servidores
Dashboard multi-usuário
Detecção de jitter mais avançada

👨‍💻 Autor

Eu 😎
Se quiser evoluir isso aqui, dá pra virar uma ferramenta MUITO forte.
