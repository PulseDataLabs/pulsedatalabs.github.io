<div align="center">
  <img src="assets/logo-full.png" alt="PulseDataLabs Logo" width="500" />
  <br><br>
  
  **Serverless Data Infrastructure for Financial Markets.**
  
  [![Pipeline Status](https://img.shields.io/badge/Data_Pipeline-Active-00d4ff?style=for-the-badge&logo=githubactions&logoColor=white)](#)
  [![Open Data](https://img.shields.io/badge/Open_Data-100%25-00d4ff?style=for-the-badge)](#)
  [![License](https://img.shields.io/badge/License-MIT-00d4ff?style=for-the-badge)](#)
  [![Format](https://img.shields.io/badge/Format-CSV_Flat_Files-4d6070?style=for-the-badge)](#)
</div>

---

A **PulseDataLabs** constrói infraestrutura de dados moderna e descentralizada para o mercado financeiro global. Automatizamos o pipeline completo de captura, normalização e versionamento de preços, indicadores econômicos e ratings de crédito. Entregamos dados limpos, estruturados e prontos para consumo com **zero fricção de infraestrutura**.

Nossa arquitetura foi desenhada para escala global, iniciando nossa cobertura pelas principais fontes e ativos do mercado brasileiro.

---

## 🚀 Nossos Produtos (Data Feeds)

### 📊 [PulseFlat](https://github.com/PulseDataLabs/PulseFlat)
Pipeline ETL serverless que captura diariamente preços de mercado e indicadores financeiros globais e regionais.
- **Fontes Iniciais:** BCB, ANBIMA, B3, CVM e IBGE.
- **Formato:** CSVs versionados no GitHub.
- **Uso:** Ideal para modelos quantitativos, backtesting e integração direta com Python/Excel.
- **Links:** [GitHub](https://github.com/PulseDataLabs/PulseFlat) · [Site](https://pulsedatalabs.github.io/PulseFlat/)

### 📈 [PulseRatings Brasil](https://github.com/PulseDataLabs/PulseRatingsBrasil)
Monitoramento automatizado e histórico consolidado de ratings de crédito corporativos e soberanos focados no mercado nacional.
- **Fontes Iniciais:** S&P Global, Moody's e Fitch.
- **Formato:** Histórico consolidado em formato Flat.
- **Uso:** Gestão de risco de crédito, compliance e análise de emissores.
- **Links:** [GitHub](https://github.com/PulseDataLabs/PulseRatingsBrasil) · [Site](https://pulsedatalabs.github.io/PulseRatingsBrasil/)

---

## ⚡ Quick Start

Consuma os dados diretamente no seu ambiente de análise:

```python
import pandas as pd

# PulseFlat — indicadores ANBIMA
url = "https://raw.githubusercontent.com/PulseDataLabs/PulseFlat/main/data/anbima_indicadores.csv"
df = pd.read_csv(url)
print(df.head())
```

```python
# PulseRatings Brasil — ratings de crédito
url = "https://raw.githubusercontent.com/PulseDataLabs/PulseRatingsBrasil/main/data/ratings.csv"
df = pd.read_csv(url)
print(df.head())
```

Todos os CSVs seguem o padrão **UTF-8, separador vírgula, decimal ponto, datas YYYY-MM-DD**.

---

## ⚙️ A Engenharia: O Padrão PulseData

Acreditamos na eficiência máxima da infraestrutura. Nossos dados não dependem de bancos de dados custosos ou APIs instáveis para a entrega do *core* aberto. Operamos baseados em um princípio simples:

`Coleta Automatizada ➔ Normalização Rígida ➔ Armazenamento Flat/Versionado ➔ Consumo Direto`

1. **Dados como Código (Data as Code):** Usamos o Git para armazenar o estado das bases em `CSV`. Isso garante um histórico imutável (*time-travel*) gratuito e auditável da evolução do mercado.
2. **Zero Infraestrutura (Serverless):** Nossos coletores rodam via GitHub Actions, garantindo previsibilidade de execução diária sem custos fixos de servidores ociosos.
3. **Fácil Integração:** Importe nossos repositórios brutos (`raw`) diretamente para o seu Pandas (`pd.read_csv()`), Power BI ou script de automação local sem a necessidade de chaves de API na versão open-source.

---

## 🌐 Roadmap e Expansão

Estamos construindo a fundação para a próxima geração de analistas quantitativos, desenvolvedores e fintechs. Embora nosso ponto de partida seja o ecossistema brasileiro, a arquitetura da PulseDataLabs está preparada para integrar feeds de mercados internacionais, pavimentando o caminho para nossas futuras soluções Enterprise e APIs de baixa latência.

---

<div align="center">
  <i>Desenvolvido com foco na eficiência. Mantido pela equipe PulseDataLabs.</i>
  <br>
  <a href="https://pulsedatalabs.github.io">Visite nosso site</a>
  <br><br>
  <a href="https://github.com/PulseDataLabs">
    <img src="https://img.shields.io/badge/GitHub-PulseDataLabs-00d4ff?style=for-the-badge&logo=github" alt="GitHub">
  </a>
</div>