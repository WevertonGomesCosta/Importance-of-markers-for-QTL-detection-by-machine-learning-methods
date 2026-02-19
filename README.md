# Importance of Markers for QTL Detection by Machine Learning Methods

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
![R](https://img.shields.io/badge/Made%20with-R-blue.svg)
![GitHub repo size](https://img.shields.io/github/repo-size/WevertonGomesCosta/Importance-of-markers-for-QTL-detection-by-machine-learning-methods)
![GitHub last commit](https://img.shields.io/github/last-commit/WevertonGomesCosta/Importance-of-markers-for-QTL-detection-by-machine-learning-methods)
[![Website](https://img.shields.io/badge/Project%20Site-online-brightgreen)](https://wevertongomescosta.github.io/Importance-of-markers-for-QTL-detection-by-machine-learning-methods/)
[![DOI](https://doi.org/10.3390/ijpb17010006)](https://doi.org/10.3390/ijpb17010006)

> **Note:** This repository contains the source code and reproducible pipeline for the research article: *"Comparison of Machine Learning Methods for Marker Identification in GWAS"*.

---

# Português

## 🧬 Sobre o Projeto

Bem-vindo ao repositório oficial. Este estudo realiza um **benchmark computacional** comparando a eficácia de métodos de **Machine Learning (ML)** contra modelos estatísticos clássicos e modernos (**Modelos Mistos / GWAS**) na identificação de marcadores moleculares (QTLs).

O pipeline integra computação de alto desempenho (HPC) para processar cenários complexos de herdabilidade e epistasia.

### 🚀 Conteúdo Principal

1.  **Genética:** Mapas de ligação e decaimento de Desequilíbrio de Ligação (LD).
2.  **GWAS Multi-Modelo:** Execução paralela de GLM, MLM, CMLM, MLMM, FarmCPU e BLINK via GAPIT.
3.  **Machine Learning:** Extração de "Feature Importance" via Random Forest, Bagging, Boosting (GBM), Decision Trees e MARS.
4.  **Consolidação:** Análise comparativa de Poder de Detecção, Precisão, Falsos Positivos e F1-Score.

### 👥 Autores

**Equipe Principal** Weverton Gomes da Costa¹, Cosme Damião Cruz², Moyses Nascimento¹*

**Afiliações** ¹ Laboratório de Inteligência Computacional e Aprendizado Estatístico (LICAE), Dep. de Estatística - UFV  
² Instituto de Inteligência Artificial e Computacional (Idata) - UFV

*\*Autor para correspondência: weverton.costa@ufv.br*
*\*Autor para correspondência: cdcruz@ufv.br*
*\*Autor para correspondência: moysesnascim@ufv.br*

### 🧭 Como Navegar no Site do Projeto

Acesse a documentação completa em: **[Project Website](https://wevertongomescosta.github.io/Importance-of-markers-for-QTL-detection-by-machine-learning-methods/)**

1.  **Genetic Map & LD:** Estrutura populacional e genômica.
2.  **Association Models:** Resultados brutos do GWAS (GAPIT) e ML.
3.  **Consolidated Analysis:** Tabelas e Heatmaps comparativos finais.

### 💻 Requisitos Técnicos

* **Linguagem:** R (≥ 4.0.0)
* **Gerenciamento de Pacotes:** `renv` (para reprodutibilidade exata).
* **Bibliotecas Chave:**
    * *GWAS:* `GAPIT`
    * *ML:* `randomForest`, `gbm`, `earth` (MARS), `rpart`, `caret`
    * *Core:* `tidyverse`, `doParallel`, `foreach`

### 📦 Instalação e Reprodução

```r
# 1. Clonar o repositório
# git clone [https://github.com/WevertonGomesCosta/Importance-of-markers-for-QTL-detection-by-machine-learning-methods.git](https://github.com/WevertonGomesCosta/Importance-of-markers-for-QTL-detection-by-machine-learning-methods.git)

# 2. Restaurar o ambiente (dentro do RStudio)
renv::restore()

# 3. Compilar o site e análises
workflowr::wflow_build()
```

-----

# English

## 🧬 About the Project

Welcome to the official repository. This study performs a **computational benchmark** comparing the efficacy of **Machine Learning (ML)** methods against classic and modern statistical models (**Mixed Models / GWAS**) in identifying molecular markers (QTLs).

The pipeline integrates high-performance computing (HPC) to process complex scenarios involving varying heritability and epistasis.

### 🚀 Core Content

1.  **Genetics:** Linkage maps and Linkage Disequilibrium (LD) decay.
2.  **Multi-Model GWAS:** Parallel execution of GLM, MLM, CMLM, MLMM, FarmCPU, and BLINK via GAPIT.
3.  **Machine Learning:** Feature Importance extraction via Random Forest, Bagging, Boosting (GBM), Decision Trees, and MARS.
4.  **Consolidation:** Comparative analysis of Detection Power, Precision, False Positive Rate, and F1-Score.

### 👥 Authors

**Core Team** Weverton Gomes da Costa¹, Cosme Damião Cruz², Moyses Nascimento¹\*

**Affiliations** ¹ Computational Intelligence and Statistical Learning Laboratory (LICAE), Statistics Dept. - UFV  
² Institute of Artificial and Computational Intelligence (Idata) - UFV

*\*Corresponding author: weverton.costa@ufv.br*
*\*Corresponding author: cdcruz@ufv.br*
*\*Corresponding author: moysesnascim@ufv.br*

### 🧭 Navigation Guide

Access the full documentation at: **[Project Website](https://wevertongomescosta.github.io/Importance-of-markers-for-QTL-detection-by-machine-learning-methods/)**

1.  **Genetic Map & LD:** Population structure and genomics.
2.  **Association Models:** Raw results from GWAS (GAPIT) and ML.
3.  **Consolidated Analysis:** Final comparative tables and Heatmaps.

### 💻 Technical Requirements

  * **Language:** R (≥ 4.0.0)
  * **Package Management:** `renv` (for exact reproducibility).
  * **Key Libraries:**
      * *GWAS:* `GAPIT`
      * *ML:* `randomForest`, `gbm`, `earth` (MARS), `rpart`, `caret`
      * *Core:* `tidyverse`, `doParallel`, `foreach`

### 📦 Installation & Reproduction

```r
# 1. Clone the repository
# git clone [https://github.com/WevertonGomesCosta/Importance-of-markers-for-QTL-detection-by-machine-learning-methods.git](https://github.com/WevertonGomesCosta/Importance-of-markers-for-QTL-detection-by-machine-learning-methods.git)

# 2. Restore environment (inside RStudio)
renv::restore()

# 3. Build website and analyses
workflowr::wflow_build()
```

-----

## ✏️ Citation / Citação

If you use this code or data, please cite:

```bibtex
@misc{costa2025importance,
  author = {Costa, Weverton Gomes and Cruz, Cosme Damião and Nascimento, Moyses},
  title = {Importance of markers for QTL detection by machine learning methods},
  year = {2025},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{[https://github.com/WevertonGomesCosta/Importance-of-markers-for-QTL-detection-by-machine-learning-methods](https://github.com/WevertonGomesCosta/Importance-of-markers-for-QTL-detection-by-machine-learning-methods)}},
  doi = {10.5281/zenodo.17866542}
}
```

## 📄 License / Licença

This work is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).  
For commercial use, please contact the authors.
