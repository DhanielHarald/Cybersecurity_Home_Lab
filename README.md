# Projeto: Meu Laboratório de Cibersegurança (Home Lab)

## 1. Objetivo

O objetivo deste projeto é criar um ambiente de rede virtual 100% isolado e controlado para praticar e estudar técnicas de cibersegurança, tanto ofensivas (Red Team) quanto defensivas (Blue Team), sem qualquer risco para a rede principal.

---

## 2. Arquitetura e Ferramentas

* **Software de Virtualização:** [VMware Workstation / VirtualBox]
* **Arquitetura de Rede:** A rede foi configurada como [ex: Host-Only / NAT] para garantir o isolamento das máquinas virtuais. Todas as VMs estão na mesma sub-rede (ex: `192.168.X.0/24`) para permitir a comunicação interna.

---

## 3. Máquinas Virtuais (VMs)

Meu laboratório é composto pelas seguintes máquinas:

### 🛡️ Máquina de Ataque (Red Team)

* **Sistema:** **Kali Linux**
* **Propósito:** Ponto central para realizar os testes de invasão. Contém todas as ferramentas necessárias (Nmap, Metasploit, Burp Suite, etc.).
* **Configuração:** Conectada à rede do laboratório.

### 🎯 Máquinas-Alvo (Sistemas Vulneráveis)

* **Sistema:** **Metasploitable 2**
    * **Propósito:** Um servidor Linux intencionalmente vulnerável, usado como alvo principal para treinar enumeração e exploração de serviços (ex: FTP, SSH, web).
* **Sistema:** **[Nome da sua outra VM, ex: Windows 7 não-atualizado]**
    * **Propósito:** Simular uma estação de trabalho de usuário final desatualizada, ideal para praticar exploração de cliente e escalação de privilégio no Windows.
* **Sistema:** **[Adicione outras VMs que você criar]**
    * **Propósito:** [Explique o propósito]

---

## 4. Próximos Passos

Os relatórios (write-ups) detalhados de cada máquina que for explorada neste laboratório serão postados em repositórios separados.
