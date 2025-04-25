# 📊 Análise Estatística da População de Cidades Brasileiras

Este projeto realiza uma análise estatística de cidades brasileiras com mais de 100 mil habitantes, com dados extraídos automaticamente da Wikipedia.  
Foram aplicadas técnicas básicas de **estatística descritiva** e **filtragem de valores extremos (outliers)** utilizando a biblioteca **Pandas** em Python.

---

## 🎯 Objetivos

- Praticar manipulação e limpeza de dados com Pandas  
- Calcular **média**, **mediana**, **moda** e **desvio padrão** da população das cidades  
- Identificar e remover **outliers** com base no desvio padrão  
- Analisar a distribuição de cidades por **Unidade Federativa (UF)**  

---

## 📌 Etapas da Análise

1. **Coleta de Dados:**  
   Uso do `pandas.read_html()` para importar tabelas diretamente da Wikipedia.

2. **Limpeza e Transformação:**  
   - Conversão da coluna de população para formato numérico  
   - Renomeação de colunas para facilitar o uso

3. **Análise Estatística (dados originais):**  
   - Cálculo de média, mediana e desvio padrão

4. **Tratamento de Outliers:**  
   - Exclusão de cidades fora da faixa de 2 desvios padrão

5. **Reanálise (dados filtrados):**  
   - Cálculo atualizado de média, mediana e moda das UFs  
   - Contagem de cidades por estado

---

## 📈 Saídas

Média (todas as cidades): 362,520
Mediana (todas as cidades): 187,315
Desvio Padrão: 792,867

Removendo cidades com população fora do intervalo [-1,223,214, 1,948,254]

Após remoção dos outliers:
Média (dados filtrados): 275,441
Mediana (dados filtrados): 183,004

Moda das UFs: SP

Contagem de cidades por UF (após filtragem):
São Paulo              77
Minas Gerais           33
Rio de Janeiro         27
Paraná                 22
Rio Grande do Sul      19
Bahia                  17
...

## 📚 Aprendizados

Este projeto reforçou habilidades como:

- Coleta de dados online com `read_html`  
- Limpeza e padronização de dados com Pandas  
- Aplicação prática de estatística descritiva  
- Identificação e tratamento de outliers  
- Análise categórica por estados brasileiros  
