# Projeto Base — Análise de Dados de Vendas

## 📌 Sobre o projeto

Projeto desenvolvido durante um desafio da DIO, com foco na consolidação e análise de dados de vendas provenientes de diferentes plataformas de terceiros.

A proposta é transformar dados brutos de vendas em informações relevantes para apoiar a fabricante de consoles na compreensão do comportamento das vendas por país e produto.

## 🏢 Contexto

### Características

- A empresa foca apenas na fabricação de consoles, deixando a distribuição e venda para terceiros.
- Os produtos são vendidos globalmente.

### Objetivos

- Consolidar diferentes bases de terceiros para realizar uma análise integrada.
- Transformar dados de vendas em informações relevantes para a fabricante.
- Identificar os produtos mais populares em cada país.
- Analisar possibilidades de otimização do processo de transporte e logística até o país de venda.

## 📂 Estrutura do projeto

A organização dos arquivos foi estruturada de forma a separar os dados brutos, os dados tratados e os materiais utilizados na etapa de análise.

```text
data/
├── process_data/
│   └── Dados tratados
│
└── raw_data/
    ├── AliExpress
    ├── Etsy
    └── Shopee

prompts/
├── Prompts utilizados
├── README
└── Insights gerados

## 📊 Dados utilizados

O projeto utiliza dados de vendas provenientes de três plataformas fictícias de terceiros, fornecidas pelo desafio de projeto:

- **AliExpress**
- **Etsy**
- **Shopee**

As bases foram disponibilizadas em arquivos CSV e posteriormente organizadas para possibilitar a consolidação e análise dos dados.

### 📁 Dados brutos

Os arquivos originais foram mantidos na pasta `data/raw_data/`, preservando as bases de origem antes do processo de tratamento.

### 📈 Dados tratados

Após o tratamento, os dados consolidados foram armazenados na pasta `data/process_data/`, permitindo sua utilização nas etapas posteriores de análise.

***As bases são fictícias e foram fornecidas pela DIO exclusivamente para a realização do desafio educacional, sendo utilizadas para fins de estudo, tratamento e análise de dados.***

## 🧹 Tratamento e organização dos dados

O processo de tratamento foi realizado a partir das três bases disponibilizadas em formato CSV, provenientes das plataformas AliExpress, Etsy e Shopee.

As bases foram consolidadas e organizadas em um único arquivo, mantendo os dados originais sem alterações em seus valores.

Durante o processo, as informações foram estruturadas em colunas para possibilitar a organização e posterior análise dos dados.

O arquivo resultante foi armazenado em `data/process_data/`, mantendo separada a base tratada das bases originais presentes em `data/raw_data/`.

## 🤖 Prompts e análise com inteligência artificial

Após a consolidação e organização dos dados, foram elaborados prompts utilizando a versão gratuita do ChatGPT como ferramenta de apoio à análise.

Os prompts foram construídos de forma progressiva, partindo de perguntas específicas sobre os dados e avançando para análises mais estratégicas.

Entre as análises realizadas estão:

- resumo de vendas por país e quantidade de unidades vendidas;
- idade média dos clientes por país e produto;
- identificação dos países com maior volume de vendas para cada produto;
- análise de quantidade vendida, faturamento e idade média dos compradores;
- relação entre produto, país, quantidade, faturamento, idade média e marketplace;
- identificação dos produtos mais populares em cada país;
- análise de possibilidades de otimização de transporte e logística.

As perguntas e respectivas respostas geradas durante o processo foram documentadas no arquivo `prompts/gptprompts.md`.

Além das respostas em formato textual e tabular, um dos insights gerados durante a análise foi apresentado também em formato visual e incluído no diretório `prompts/`.

### 💡 Processo de análise

O processo seguiu, de forma geral, o fluxo:

**Dados consolidados → Formulação dos prompts → Respostas geradas → Análise dos resultados → Insights**

A utilização da inteligência artificial teve como objetivo apoiar a transformação dos dados consolidados em informações que pudessem responder aos objetivos definidos para o desafio.

## 💡 Insights gerados

A análise dos dados permitiu identificar padrões de vendas por produto, país e marketplace, além de diferenças no perfil dos clientes.

Entre os principais insights observados:

- concentração de determinados produtos em mercados específicos;
- identificação dos principais países para cada produto;
- diferenças na idade média dos compradores entre os mercados;
- distribuição das vendas entre diferentes marketplaces;
- identificação de oportunidades para direcionamento de estoque e planejamento logístico.

Um dos insights gerados durante o processo também foi apresentado em formato visual:

![Insight gerado pelo ChatGPT](prompts/Unidades%20vendidas%20por%20pa%C3%ADs%20-%20INSIGHT%20GERADO%20PELO%20CHAT%20GPT.png)

Os resultados apresentados refletem exclusivamente os dados fictícios fornecidos pela DIO para o desafio.

## 🛠️ Ferramentas utilizadas

- **Visual Studio Code** — organização e documentação do projeto
- **Excel** — consolidação e organização dos dados
- **ChatGPT** — elaboração de prompts e apoio à análise dos dados
- **Git e GitHub** — versionamento e publicação do projeto
