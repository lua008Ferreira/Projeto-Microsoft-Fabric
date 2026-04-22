#Projeto de Estudos Microsoft Fabric - DP-600
##Módulo 1: Ingestão e Lakehause (Arquitetura Medallion)
| Camada | Descrição no Fabric | Status do Dado |
| Camada | Descrição no Fabric | Status do Dado |
| :--- | :--- | :--- |
| 🥉 **Bronze** | Ingestão direta (Pipelines/Shortcuts) | Raw |
| 🥈 **Silver** | Limpeza e Integração (Notebooks) | Cleansed |
| 🥇 **Gold** | Modelos de Negócio (Star Schema) | Curated |
### O 'Balde' da Camada Bronze 🪣
Nesta fase, coletamos os dados brutos. O objetivo é a **ingestão rápida** e a **fidelidade** ao dado original.
#### Como os dados entram no 'Balde'? 📥
* 🏗️ **Copy Activity (Pipelines):** Move uma **cópia** física do dado da fonte para o Lakehouse.
* 🔗 **Shortcuts (Atalhos):** Cria um **link** para o dado onde ele já está, sem movê-lo de verdade.
  ### O 'Balde' da Camada Bronze (Ingestão) 🪣

Nesta fase, coletamos os dados brutos. O objetivo é a **ingestão rápida** e a **fidelidade** ao dado original.

Aqui estão os dados como eles chegaram: misturados e guardados no formato **Delta/Parquet**.
---

## Módulo 2: OneLake - O OneDrive dos Dados 🌐

O **OneLake** é o sistema de armazenamento único e lógico para toda a organização. No Microsoft Fabric, todos os dados residem em um único lugar, eliminando silos.

### 🏠 Características do OneLake:
* **Um só lugar:** Todos os workspaces compartilham o mesmo armazenamento.
* **Aberto:** Baseado no formato **Delta Lake** (Parquet), permitindo que qualquer ferramenta compatível o acesse.
* **Seguro:** Governança centralizada para todos os seus dados.

![O Balde de Dados Brutos (Camada Bronze)](https://i.imgur.com/eG1M5O0.png)

