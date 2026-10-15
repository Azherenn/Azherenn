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
    const char *foco;
    const char *cursando;
    const char *aberto_a;
} Magno;

int main(void) {
    Magno eu = {
        .nome     = "Magno (Azherenn)",
        .base     = "Rio de Janeiro, RJ",
        .foco     = "C, redes e segurança defensiva",
        .cursando = "Engenharia de Software (2026-2030)",
        .aberto_a = "estágio / Jovem Aprendiz em TI e cibersegurança",
    };

    printf("Olá, mundo! Eu sou o %s.\n", eu.nome);
    return 0;
}
```

Sou técnico em **Informática** e em **Telecomunicações** (FAETEC) e estudo **Engenharia de Software**. Gosto de entender o que acontece por baixo das abstrações: pacotes na rede, memória, sockets, sinais em fibra óptica. Hoje coloco isso em prática em projetos de segurança defensiva e de desempenho.

## 📊 Em números

| | |
|:---:|:---:|
| **1 milhão+** | registros processados no projeto Python + C |
| **~20x** | ganho de desempenho sobre Pandas/NumPy |
| **Top 100** | 12ª Maratona CiberEducação Cisco (CTF) |
| **100+** | relatórios padronizados que consolidei como Jovem Aprendiz |

## 🚀 Projetos

### 🛡️ [c-ids](https://github.com/Azherenn/c-ids) · IDS/IPS em C `em desenvolvimento`

Sistema de detecção e prevenção de intrusão feito do zero em C, para estudar redes, captura de pacotes e detecção de tráfego suspeito.

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

### ⚡ [High-Performance-Data-Processing](https://github.com/Azherenn/High-Performance-Data-Processing) · Python + C

Sistema em três camadas que processa e analisa mais de 1 milhão de registros. Python orquestra, o motor de cálculo em C é compilado como *shared library* e os dados ficam em SQLite. Resultado: cerca de **20x** mais rápido que a implementação nativa com Pandas/NumPy.

**Stack:** Python · C · SQLite · Pandas · NumPy

<details>
<summary><b>Arquitetura</b></summary>

```mermaid
flowchart TB
    P["Python<br/>orquestração"] --> C["Motor de cálculo em C<br/>shared library"]
    P --> D[("SQLite<br/>dados")]
```

</details>

### 🎮 [Hangman-Game](https://github.com/Azherenn/Hangman-Game) · Jogo da forca em C

Jogo de linha de comando feito do zero para praticar os fundamentos da linguagem e criar uma experiência interativa no terminal.

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

## 🎓 Formação e certificações

| | |
|---|---|
| 🎓 **Engenharia de Software** | Gran Faculdade · 2026 a 2030 (previsão) |
| 📡 **Técnico em Telecomunicações** | FAETEC, Escola Técnica Ferreira Viana · 2024 a 2025 |
| 💻 **Técnico em Informática** | FAETEC, Escola Técnica Rezende de Rammel · 2020 a 2023 |
| 🔐 **CCEP** | Certified Cybersecurity Educator Professional, Red Team Leaders · 04/2026 |
| 🛡️ **Cisco CyberOps Associate** | Curso concluído · 06/2026 (e curso Cisco Ethical Hacker) |
| 🏆 **Maratona CiberEducação Cisco** | 12ª edição, CTF · Top 100 individual |
| ⚙️ **NVIDIA** | Lab de inferência de IA em GPU com PyTorch (Tesla T4) · 11/2025 |
| 🤖 **Alura** | Trilha de IA Generativa · 20 de 30 cursos |

## 📚 Estudando agora

- C com foco em resolução de problemas e estruturas de dados
- Evolução do **c-ids**
- Python, Ruby e IA generativa (LangChain/RAG, Hugging Face)

## 📫 Vamos conversar?

Estou buscando estágio ou vaga de Jovem Aprendiz em TI, com foco em cibersegurança.

<div align="center">

<a href="https://www.linkedin.com/in/magno-ferreira-ti/"><img src="https://img.shields.io/badge/Me_chame_no-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>

<br/><br/>

<i>Construindo software confiável, uma camada de cada vez.</i>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:1f6feb&height=100&section=footer" alt="Rodapé" width="100%"/>

</div>
