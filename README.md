# Projeto-Tableau-Receita-de-Faturamento

## 🚩 Desafio
Como analista, identifiquei que a empresa possui uma operação robusta, mas enfrentava dificuldades para visualizar quais setores e regiões eram realmente rentáveis. O tempo de recebimento e o volume de faturamento variavam drasticamente entre as zonas, dificultando a identificação de perdas e ganhos reais.

## 🎯 Objetivo
Desenvolver um painel analítico que resuma a operação, permitindo visualizar **custos, lucro e faturamento**. O foco é transformar dados brutos em indicadores de margem média e performance regional para suporte estratégico à tomada de decisão.

## 🛠️ Tecnologias Utilizadas
* **Tableau**: Visualização de dados e Storytelling.
* **Excel: Manipulação da base de dados de faturamento.

---

## 📈 Etapa 1: Engenharia de Dados & Cálculos

Nesta etapa, foi criada a inteligência por trás dos gráficos utilizando campos calculados avançados:

* **Cálculo de Lucro Real**: Implementação da métrica de lucro total subtraindo o importe do fornecedor do importe do cliente.
    > `SUM([Importe Cliente]) - SUM([Importe Fornecedor])`
* **Diferenciação de Status**: Criação de lógica condicional para identificar pagamentos realizados (**Sim**) vs. pendências (**Não pago**), garantindo a integridade da soma do faturamento.
* **KPI de Margem Média**: Desenvolvimento de cálculo para medir quanto cada real investido nos cursos retornou como ganho efetivo para a empresa.

## 📊 Etapa 2: Business Intelligence (Tableau)

Os dados foram organizados para uma leitura rápida e intuitiva através de:

1.  **Ranking de Setores**: Aplicação de filtros de *Top N* e parâmetros para identificar os setores com maior lucratividade e volume pago.
2.  **Análise Geográfica**: Mapeamento da quantidade de faturas por províncias, com foco em regiões-chave como **Barcelona, Madrid e Alicante**.
3.  **Interface Interativa**: Design limpo com KPIs em destaque (Lucro Total, Custo, Faturamento e Médias) para uma visão 360º da saúde financeira.

Visualização:
<img width="532" height="323" alt="image" src="https://github.com/user-attachments/assets/1c9889a3-32c4-4bca-9446-fff0d124494f" />


---

## 🚀 Resultados Obtidos
* **Transparência Financeira**: Identificação clara de onde o lucro está sendo retido e onde a operação é mais eficiente.
* **Visão Regional**: O gestor agora consegue comparar o desempenho entre províncias através do mapa interativo.
* **Agilidade na Análise**: Substituição de relatórios estáticos por um painel dinâmico que diferencia automaticamente o que foi pago do que ainda é custo.
