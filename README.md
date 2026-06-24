# Vendas, Logística e Satisfação no E-commerce (Olist)

Solução de Business Intelligence de ponta a ponta baseada no dataset público da Olist[cite: 2].

## O Problema de Negócio
Identificar onde a operação concentra problemas de prazo e satisfação de clientes[cite: 2]. O foco é entender quais regiões, categorias e vendedores priorizar para reduzir atrasos e aumentar a recompra[cite: 2].

## Principais Indicadores (KPIs)
O dashboard acompanha sete métricas[cite: 2]:
* **Receita Total (GMV):** Resultado financeiro central[cite: 2].
* **Ticket Médio:** Valor gasto por compra[cite: 2].
* **Prazo Médio de Entrega:** Tempo entre a compra e a entrega[cite: 2].
* **Taxa de Atraso:** Pedidos entregues após a estimativa[cite: 2].
* **Nota Média:** Avaliação dos clientes (1 a 5)[cite: 2].
* **Taxa de Recompra:** Clientes com duas ou mais compras[cite: 2].
* **% Frete sobre Receita:** Peso do custo de envio no faturamento[cite: 2].

## Modelagem de Dados e Arquitetura
Os dados de oito tabelas "flat" foram tratados no Power Query e estruturados em modelo dimensional constelação[cite: 2]:
* **Tabelas Fato:** `fato_itens` (item do pedido) e `fato_pedidos` (pedido total)[cite: 2].
* **Tabelas Dimensão:** `dCalendario`, `dCliente`, `dProduto` e `dVendedor`[cite: 2].

Foram criadas 17 medidas em DAX e implementado Row-Level Security (RLS) para os perfis: Diretoria, Gerente Sudeste e Gerente Sul[cite: 2].

## Estrutura do Dashboard
O relatório possui três páginas[cite: 2]:
1. **Visão Executiva:** Resumo dos KPIs e evolução temporal[cite: 2].
2. **Análise de Vendas e Produtos:** Desempenho por categoria (Top 10), relação preço x frete e matriz regional[cite: 2].
3. **Logística e Satisfação:** Prazos, taxas de atraso e relação com notas e recompra[cite: 2].

## O Dataset
* **Fonte:** Brazilian E-Commerce Public Dataset by Olist (Kaggle)[cite: 2].
* **Volume:** ~100 mil pedidos (set/2016 a out/2018)[cite: 2].
* Link e licença no arquivo `data/README.md`[cite: 2].

## Como Executar o Projeto
1. Instale a versão mais recente do **Power BI Desktop**[cite: 2].
2. Abra o arquivo `pbip/ecommerce_olist.pbip`[cite: 2].

---
**Autor:** Mateus Itibal[cite: 2]
**Contexto Acadêmico:** Projeto Final de Business Intelligence II - CEUB[cite: 2]
