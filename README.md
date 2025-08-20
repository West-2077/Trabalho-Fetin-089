#Trabalho-Fetin-089 — Automação de Respostas a Alertas do Wazuh
!Status
!Docker
!Wazuh


---

##📌 Sobre o Projeto
Este projeto monitora os alertas gerados pelo SIEM Wazuh em tempo real e executa respostas automáticas com base no tipo e nível do alerta.

---

##📜 Funcionalidades
-📄 Leitura e análise do arquivo alerts.json em tempo real.
-🚫 Ações automáticas como bloqueio de IP malicioso.
-📝 Registro de incidentes para auditoria e acompanhamento.

---

##🐳 Instalação do Wazuh com Docker
O projeto utiliza a imagem oficial do Wazuh para criar um ambiente de SIEM local.

Componentes Utilizados
wazuh/wazuh-manager — Gerenciamento de agentes e regras.
wazuh/wazuh-indexer — Armazenamento e indexação de logs e alertas.
wazuh/wazuh-dashboard — Interface gráfica para análise e visualização.

---

📚 Documentação Oficial
Documentação Wazuh - Docker
Repositório Oficial no GitHub

---

⚙️ Etapas de Instalação
Instale o Docker Desktop
Download Docker Desktop

Clone este repositório
```bash
git clone https://github.com/seu-usuario/Trabalho-Fetin-089.git
cd Trabalho-Fetin-089
Suba os containers```bash
docker-compose up -d

Acesse o painel Wazuh
http://localhost:5601/

🚀 Execução da Automação
Quando o Wazuh estiver rodando, o script de automação ficará monitorando alerts.json e:

Detectará alertas críticos.

Executará respostas automáticas (como bloqueio de IP).

Registrará eventos para auditoria.
