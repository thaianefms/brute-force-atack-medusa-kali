# Desafio de Projeto #1 do curso da DIO Santander Cibersegurança 2025

## Brute Force Attack Simulation with Medusa (Kali Linux)

Este repositório documenta o processo de simulação de um ataque de força bruta utilizando a ferramenta **Medusa** em um ambiente controlado no **Kali Linux**, realizado em outubro de 2025. O objetivo deste material é puramente educacional e focado em testes de segurança defensiva e análise de vulnerabilidades em serviços de rede.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas
* **Sistema Operacional:** Kali Linux
* **Ferramenta de Teste:** Medusa (Brute Force Credential Testing)
* **Documentação:** Capturas de tela e logs de execução

---

## 📂 Estrutura do Repositório

```text
├── README.md                                   # Documentação principal do repositório
└── brute-force-atack-medusa-kali-.../          # Diretório contendo evidências e capturas
    ├── Screenshot_2025-10-24_13_09_52.png      # Configuração inicial / Alvo
    ├── Screenshot_2025-10-24_13_16_30.png      # Execução do ataque (Medusa)
    ├── Screenshot_2025-10-24_13_18_48.png      # Carregamento de wordlists
    ├── Screenshot_2025-10-24_13_28_29.png      # Parâmetros de conexões simultâneas
    ├── Screenshot_2025-10-24_13_30_19.png      # Monitoramento de tráfego/respostas
    ├── Screenshot_2025-10-24_13_31_05.png      # Tentativas de autenticação
    ├── Screenshot_2025-10-24_13_35_12.png      # Validação de credenciais
    ├── Screenshot_2025-10-24_13_37_12.png      # Resultados parciais
    ├── Screenshot_2025-10-24_13_44_40.png      # Identificação de credencial válida (Match)
    └── Screenshot_2025-10-24_13_47_47.png      # Relatório final e encerramento
```

### 🔍 Sobre a Simulação
O projeto demonstra a eficiência de ataques de força bruta baseados em dicionário (wordlists) contra serviços de autenticação de rede. O Medusa foi selecionado devido à sua alta velocidade e suporte a conexões paralelas via threads, permitindo testar múltiplos pares de usuário e senha de forma simultânea.

**Principais Fases Registradas nas Evidências:**
* **Mapeamento do Alvo:** Identificação do serviço exposto e portas ativas.
* **Definição de Dicionários:** Configuração de listas de usuários e senhas potenciais.
* **Execução Paralela:** Disparo das requisições de login via Medusa otimizando o uso de threads.
* **Análise de Resposta:** Identificação de falsos positivos e captura bem-sucedida de credenciais válidas.

---

### 🛡️ Considerações de Segurança & Mitigação
Ataques de força bruta representam riscos críticos para sistemas expostos à internet. Algumas das principais práticas de mitigação incluem:

* **Políticas de Senhas Fortes:** Exigir senhas complexas e longas para mitigar a eficácia de ataques de dicionário.
* **Limitação de Tentativas (Rate Limiting):** Bloquear temporariamente endereços IP após um número excedente de falhas consecutivas de login.
* **Autenticação Multifator (MFA):** Adicionar uma camada extra de segurança que impede o acesso mesmo em caso de comprometimento da senha única.
* **Uso de Soluções de Monitoramento (IDS/IPS):** Detectar picos anômalos de requisições de autenticação na rede.

---

### ⚠️ Aviso Legal (Disclaimer)
> Este material foi desenvolvido estritamente para fins educacionais e de pesquisa em segurança da informação. A execução de ataques de força bruta contra sistemas sem a autorização prévia e explícita do proprietário é ilegal e antiética. O autor não se responsabiliza pelo uso indevido destas informações.

