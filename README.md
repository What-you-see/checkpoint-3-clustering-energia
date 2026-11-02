# Checkpoint 3 — Clustering Aplicado à Energia

Repositório dedicado à atividade prática de Machine Learning não supervisionado utilizando o algoritmo **K-Means**, Método Elbow e Silhouette Score para segmentação de perfis de unidades consumidoras de energia.

## 👥 Integrantes e RM
* Nome: Pedro Vianna — RM: 570747


## 🎯 Objetivo da Atividade
Identificar grupos de unidades consumidoras com comportamentos semelhantes a partir de dados de consumo mensal, demanda máxima e percentual de consumo noturno, auxiliando a equipe de gestão de energia no planejamento de ações direcionadas.

## 📊 Descrição da Base de Dados
A base contém 120 unidades consumidoras fictícias com as seguintes variáveis:
* `id_unidade`: Identificador da unidade (excluído do modelo).
* `consumo_mensal_kwh`: Energia total consumida no mês (kWh).
* `demanda_maxima_kw`: Maior demanda de potência registrada em uma janela de 15 minutos no mês (kW).
* `consumo_noturno_pct`: Parcela da energia mensal consumida entre 18h e 6h (% de 0 a 100).

## ⚙️ Instruções para Executar o Notebook
1. Faça o download do arquivo `Checkpoint_3_Clustering.ipynb` contido neste repositório.
2. Acesse o [Google Colab](https://colab.research.google.com/).
3. Faça o upload do notebook (`Arquivo > fazer upload do notebook`).
4. Como a base de dados já está incorporada diretamente no código do notebook, basta ir em **Ambiente de execução** e clicar em **Executar tudo**.

## 🚀 Principais Resultados Encontrados
* **Padronização:** Utilizado o `StandardScaler` para equiparar as escalas das variáveis.
* **Método Elbow:** Apontou uma clara inflexão em **$k = 3$ clusters**.
* **Silhouette Score:** Corroborou a escolha de 3 grupos, garantindo uma boa coesão interna e separação entre os perfis.
* **Perfis Identificados:** A segmentação permitiu separar os consumidores em grupos distintos de comportamento (como consumo padrão, alta demanda e perfil noturno), viabilizando estratégias tarifárias e operacionais específicas.
