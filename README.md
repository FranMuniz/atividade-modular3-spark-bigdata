## 🧠 Atividade Modular – Módulo 3: Soluções de Big Data e Data Lake

Este repositório contém a solução desenvolvida para a **Atividade Modular do Módulo 3** da Pós-graduação em Engenharia de Dados, ministrada pelo [Prof. Pedro Calais](https://www.linkedin.com/in/pedrohcalais/).

### 📚 Objetivos da Atividade

Exercitar, na prática, os seguintes conceitos fundamentais do ecossistema de Big Data com Apache Spark:

- 📄 **Spark SQL** para consultas e manipulação de dados  
- 🧩 **UDFs (User Defined Functions)** para tratamento e enriquecimento de dados  
- 🧱 **Formato Parquet**, um dos mais utilizados para armazenar dados em Data Lakes  
- ⚙️ Conhecimentos gerais sobre o uso do **Apache Spark**

---

### 📦 Conjuntos de Dados Utilizados

Os dados utilizados foram obtidos a partir do seguinte repositório público:

🔗 [http://www.dcc.ufmg.br/~pcalais/XPE/engenharia-dados/big-data-spark/desafio](http://www.dcc.ufmg.br/~pcalais/XPE/engenharia-dados/big-data-spark/desafio)

### 1. CNAEs  
Contém os códigos CNAE (Classificação Nacional de Atividades Econômicas) e suas respectivas descrições, como por exemplo:  
> `0116403` → *"Cultivo de Mamona"*

### 2. Estabelecimentos  
Informações detalhadas sobre os estabelecimentos brasileiros, como:  
- CNPJ  
- Código CNAE  
- Endereço  
- Telefone  
- Situação cadastral  
*(Esquema de dados disponível no arquivo `NOVOLAYOUTDOSDADOSABERTOSDOCNPJ.pdf`)*

---

### ❓ Perguntas a serem respondidas 

1. Quantos estabelecimentos existem?  
2. Na tabela de estabelecimentos, quantas colunas existem e quantas são identificadas pelo Spark como números? Use o `inferSchema` ao ler os arquivos.  
3. Comparando o tamanho do(s) arquivo(s) CSV original(is) com o arquivo Parquet gerado pelo Spark (`estabelecimentos.parquet`), qual é a economia de espaço obtida?  
4. Quantos estabelecimentos não têm logradouro cadastrado?  
5. Quantos estabelecimentos têm um logradouro cujo endereço está incorretamente preenchido com "AVENIDA" na coluna `LOGRADOURO`?  
6. Quantos CEPs distintos existem entre os estabelecimentos?  
7. Quantos CNAEs existem na tabela de CNAEs?  
8. Quantos estabelecimentos possuem um CNAE relacionado a cultivo?  
9. Quantos estabelecimentos são filiais?  

---

### 🔧 O que foi feito

- Leitura dos arquivos com **Spark SQL**  
- Criação de **UDFs** para processar e enriquecer os dados  
- Conversão e persistência em **formato Parquet**  
- Resolução das perguntas propostas usando SQL distribuído  
- Organização do código com foco em clareza e reprodutibilidade  

---

### 🧪 Como executar

Certifique-se de que você possui o Apache Spark instalado em sua máquina ou utilize soluções como o Google Colab.
