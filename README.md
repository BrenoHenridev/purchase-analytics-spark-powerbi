# Análise de Compras com Spark e Power BI

## Visão Geral
Este projeto apresenta um **pipeline de dados de ponta a ponta** para análise de compras, utilizando **Apache Spark (Databricks)** para ingestão e transformação dos dados e **Power BI** para consumo analítico e visualização.

O objetivo é simular um cenário real de Analytics, aplicando a arquitetura **Bronze / Silver / Gold** e entregando insights de negócio por meio de um dashboard interativo.

---

## Arquitetura do Projeto
O projeto segue uma arquitetura em camadas, amplamente utilizada em ambientes de dados modernos:

- **Bronze**: ingestão dos dados brutos
- **Silver**: limpeza, padronização e tipagem dos dados
- **Gold**: camada analítica pronta para consumo

Fluxo simplificado:

Databricks (Spark)  
→ Bronze  
→ Silver  
→ Gold  
→ Power BI

---

## Tecnologias Utilizadas
- **Apache Spark (PySpark)** – processamento de dados
- **Databricks** – ambiente de execução em nuvem
- **Power BI** – visualização e análise de dados
- **GitHub** – versionamento e documentação

---

## Estrutura do Repositório
purchase-analytics-spark-powerbi/
├── cloud/
│   ├── bronze_compras.ipynb
│   ├── silver_compras.ipynb
│   └── gold_compras.ipynb
├── powerbi/
│   ├── ProjetoPBI.pbix
│   └── image.png
└── README.md


---

## Dashboard no Power BI
O dashboard foi desenvolvido para fornecer uma visão executiva e analítica das compras, contemplando:

- Valor total de compras
- Variação mês a mês (MoM)
- Quantidade de compras e itens vendidos
- Evolução do valor ao longo do tempo
- Distribuição por status (Entregue, Em trânsito, Cancelado)
- Produtos e fornecedores com maior valor

Prévia do dashboard:

![Dashboard de Compras](powerbi/image.png)


---

## Principais Destaques
- Pipeline de dados completo (end-to-end)
- Separação clara entre ingestão, tratamento e consumo
- Transformações realizadas em Spark com foco analítico
- Dashboard orientado a indicadores de negócio
