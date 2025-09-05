# Projeto: Limpeza e Análise de Dados com Python

Este projeto é um exemplo prático de como pegar um **dataset bruto e desorganizado** e prepará-lo para análise. O objetivo foi aplicar técnicas essenciais de pré-processamento de dados para garantir que as informações fossem consistentes e confiáveis.

---

### Etapas do Processo

1.  **Carregamento e Exploração Inicial**
    * Comecei carregando o dataset (`atividade3_dataset.csv`) e fazendo uma exploração rápida para entender sua estrutura, tipos de dados e identificar problemas iniciais, como valores ausentes e inconsistências.

2.  **Limpeza e Padronização de Dados**
    * **Padronização de Cidades:** Consertei os nomes das cidades para que "são paulo" e "SÃO PAULO" fossem tratados da mesma forma, garantindo que a contagem estivesse correta.
    * **Conversão de Tipos:** Transformei colunas como `Preço` e `Idade` de texto para número, corrigindo as vírgulas no preço. A coluna `Data_Compra` foi convertida para o formato de data.

3.  **Tratamento de Valores Ausentes**
    * Lidei com os dados faltantes de forma estratégica:
        * **Idade:** Preenchi com a **mediana**, que é uma medida mais segura e não é influenciada por valores discrepantes (outliers).
        * **Preço:** Preenchi com a **média** para manter a distribuição do dataset.
        * **Produto:** Usei o valor **"Desconhecido"**, pois não era possível inferir o nome do produto.

4.  **Remoção de Duplicatas**
    * Verifiquei e eliminei todas as linhas duplicadas para garantir que cada registro fosse único, o que é fundamental para não distorcer a análise estatística.

5.  **Análise e Visualização Inicial**
    * Com o dataset limpo, realizei uma análise exploratória básica. Gerei dois gráficos simples para visualizar a distribuição das idades e a relação entre preço e quantidade.

---

### Tecnologias Utilizadas

* **Python**: Linguagem de programação.
* **Pandas**: Biblioteca para manipulação e análise de dados.
* **Matplotlib e Seaborn**: Bibliotecas para visualização de dados.
