<!-- ============ CABEÇALHO ============ -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:1f6feb&height=190&section=header&text=Magno%20(Azherenn)&fontSize=42&fontColor=ffffff&fontAlignY=36&desc=C%20%C2%B7%20Redes%20%C2%B7%20Seguran%C3%A7a%20Defensiva&descSize=18&descAlignY=58" alt="Cabeçalho" width="100%"/>

<a href="https://github.com/Azherenn">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=1200&color=58A6FF&center=true&vCenter=true&width=620&height=40&lines=T%C3%A9cnico+em+Inform%C3%A1tica+e+Telecom;Estudante+de+Engenharia+de+Software;Construindo+um+IDS%2FIPS+em+C;Blue+team+em+forma%C3%A7%C3%A3o" alt="Texto animado" />
</a>

<br/>

<a href="https://www.linkedin.com/in/magno-ferreira-ti/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<img src="https://img.shields.io/badge/Rio_de_Janeiro-RJ-1f6feb?style=for-the-badge" alt="Rio de Janeiro"/>
<img src="https://img.shields.io/badge/Aberto_a-Est%C3%A1gio_em_TI-2ea043?style=for-the-badge" alt="Aberto a estágio em TI"/>

</div>

---

## `$ whoami`

```c
#include <stdio.h>

typedef struct {
    const char *nome;
    const char *base;
    const char *formacao;
    const char *foco;
    const char *estudando;
    const char *aberto_a;
} Magno;

int main(void) {
    Magno eu = {
        .nome      = "Magno (Azherenn)",
        .base      = "Rio de Janeiro, RJ",
        .formacao  = "Técnico em Informática e Telecom + Engenharia de Software",
        .foco      = "C, redes e segurança defensiva",
        .estudando = "ponteiros, tráfego de rede e IA generativa",
        .aberto_a  = "estágio / Jovem Aprendiz em TI e cibersegurança",
    };

    printf("Olá, mundo! Eu sou o %s.\n", eu.nome);
    return 0;
}
```

Minha história começou na **camada física**: no técnico de Telecom eu calculava perdas de sinal em fibra óptica. Depois fui subindo, para redes, programação e segurança. Hoje o que me move é entender **o que acontece por baixo das abstrações**, desde o sinal no cabo até o pacote que chega ao servidor, e usar isso para **defender redes**.

## 📊 Em números

| | |
|:---:|:---|
| **1 milhão+** | de registros de vendas processados no [Sales Performance Analyzer](https://github.com/Azherenn/High-Performance-Data-Processing) (Python + C) |
| **~20x** | mais rápido que Pandas no cálculo estatístico desse mesmo projeto |
| **Top 100** | na 12ª Maratona CiberEducação Cisco (CTF) |
| **100+** | relatórios padronizados que consolidei como Jovem Aprendiz na Atento |

## 🚀 Projetos

### 🛡️ [c-ids](https://github.com/Azherenn/c-ids) · IDS/IPS em C `em desenvolvimento`

Sistema de detecção e prevenção de intrusão feito do zero em C, para entender de verdade como captura de pacotes e detecção de tráfego suspeito funcionam, em vez de usar o Snort ou o Suricata como caixa-preta. É o **primeiro de cinco projetos** do meu roadmap blue team: IDS → Honeypot → Integração → Análise de TLS → EDR com eBPF.

Hoje estou nos fundamentos que vêm antes do parser de pacotes: manipulação de bytes, layout de memória e aritmética de ponteiros.

**Stack:** C · raw sockets · iptables · MySQL · GCC/Make · Linux

<details>
<summary><b>Arquitetura alvo</b></summary>

```mermaid
flowchart LR
    T([Tráfego de rede]) --> S[Raw socket<br/>captura de pacotes]
    S --> A[Análise<br/>de pacotes]
    A -->|tráfego suspeito| I[iptables<br/>resposta]
    A --> L[(MySQL<br/>log de eventos)]
    I --> L
```

</details>

### ⚡ [Sales Performance Analyzer](https://github.com/Azherenn/High-Performance-Data-Processing) · Python + C

Feito em dupla com o Ricardo. Python é ótimo para gerenciar dados e lento em matemática pesada, então a conta fica numa biblioteca compartilhada em C, chamada pelo Python via `ctypes`. Processa **1 milhão de vendas** guardadas em SQLite e calcula total, média e desvio padrão em **1,6 ms**, contra 33,7 ms do Pandas (**~20x**).

**Stack:** Python · C · SQLite · ctypes · Pandas · NumPy

<details>
<summary><b>Arquitetura</b></summary>

```mermaid
flowchart LR
    D[("SQLite<br/>1M de vendas")] -->|extrai| P["Python<br/>orquestra e mede"]
    P -->|ponteiros via ctypes| C["Biblioteca em C<br/>total, média, desvio padrão"]
```

</details>

### 🎮 [Hangman-Game](https://github.com/Azherenn/Hangman-Game) · Jogo da forca em C

Jogo de terminal que roda em Windows e Linux (detecta o sistema com `#ifdef`), lê palavras, dicas e níveis de um arquivo externo e desenha a forca em ASCII. Foi onde pratiquei structs, ponteiros e leitura de arquivos.

**Stack:** C

### 📡 TCC de Telecomunicações · Enlace de fibra óptica RJ ↔ BH

Dimensionamento de um enlace óptico de longa distância entre Rio de Janeiro e Belo Horizonte, com orçamento de potência e balanço de perdas para validar a viabilidade da rede. Automatizei em Excel as análises de atenuação e dispersão.

## 🛠️ Tecnologias

**Linguagens e dados**<br/>
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Ruby](https://img.shields.io/badge/Ruby_(estudando)-CC342D?style=flat-square&logo=ruby&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)

**Segurança e redes**<br/>
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white)
![Nmap](https://img.shields.io/badge/Nmap-4682B4?style=flat-square)
![iptables](https://img.shields.io/badge/iptables-E95420?style=flat-square)
![TCP/IP](https://img.shields.io/badge/TCP%2FIP-1f6feb?style=flat-square)
![DNS](https://img.shields.io/badge/DNS-1f6feb?style=flat-square)
![VPN](https://img.shields.io/badge/VPN-1f6feb?style=flat-square)
![Firewall](https://img.shields.io/badge/Firewall-1f6feb?style=flat-square)
![CTF](https://img.shields.io/badge/CTF-8957e5?style=flat-square)

**Ferramentas**<br/>
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=flat-square&logo=ubuntu&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GCC](https://img.shields.io/badge/GCC%20%2F%20Make-A42E2B?style=flat-square&logo=gnu&logoColor=white)
![Jira](https://img.shields.io/badge/Jira-0052CC?style=flat-square&logo=jira&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)

**IA e computação em GPU**<br/>
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white)

**Idiomas:** Português (nativo) · Inglês (B1)

## 🧭 Trajetória

```mermaid
timeline
    title Minha jornada
    2020 : Início do Técnico em Informática na FAETEC
    2023 : Conclusão do Técnico em Informática
    2024 : Técnico em Telecomunicações na FAETEC : Jovem Aprendiz em Planejamento na Atento
    2025 : TCC com enlace de fibra óptica RJ a BH : Lab NVIDIA de inferência em GPU : DevFest Rio : Conclusão de Telecom
    2026 : Top 100 na Maratona Cisco CTF : Aprovação no CCEP : Curso Cisco CyberOps Associate : Início de Engenharia de Software
    2030 : Previsão de formatura
```

## 🏆 Certificações e conquistas

- 🔐 **CCEP**: Certified Cybersecurity Educator Professional, Red Team Leaders (04/2026)
- 🛡️ **Cisco CyberOps Associate** (curso concluído, 06/2026) e **Cisco Ethical Hacker** (curso)
- 🥇 **Top 100** individual na 12ª Maratona CiberEducação Cisco (CTF)

## 📚 Estudando agora

- 💻 **C**: ponteiros, memória dinâmica e estruturas de dados, com exercícios todos os dias
- 🛡️ **c-ids**: fundamentos de bytes e memória antes do parser de pacotes
- 🛰️ **Cisco**: próximo passo da trilha, do CyberOps Associate rumo ao Professional
- 🤖 **IA generativa** (trilha da Alura): `▰▰▰▰▰▰▱▱▱▱` 20 de 30 cursos, com LangChain/RAG, Hugging Face e n8n
- ⚙️ **Inferência em GPU**: lab da NVIDIA com PyTorch (Tesla T4) concluído em 11/2025
- 💎 **Ruby**: primeiros passos

## 📫 Vamos conversar?

Estou buscando estágio ou vaga de Jovem Aprendiz em TI, com foco em cibersegurança. Se você trabalha com redes, segurança defensiva ou C, vou gostar de trocar uma ideia.

<div align="center">

<a href="https://www.linkedin.com/in/magno-ferreira-ti/"><img src="https://img.shields.io/badge/Me_chame_no-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>

<br/><br/>

<i>Construindo software confiável, uma camada de cada vez.</i>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:1f6feb&height=100&section=footer" alt="Rodapé" width="100%"/>

</div>
