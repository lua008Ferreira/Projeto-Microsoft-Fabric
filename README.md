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


