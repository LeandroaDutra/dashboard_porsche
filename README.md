[index.html.html](https://github.com/user-attachments/files/33455903/index.html.html)# dashboard_porsche
Criada dashboard de vendas da marca porsche 
## Dashboard de Vendas Porsche: descrição

**Perguntas de negócio e por quê**
As cinco perguntas que foram definidas serve a uma decisão comercial:
- **Principais modelos por estado e modelo líder em cada estado:** mostram onde cada modelo tem mais demanda, o que ajuda a distribuir estoque e esforço de venda.
- **Ano de modelo mais vendido no período:** mostra se a demanda está em carros mais novos ou mais antigos.
- **Modelos populares por cidade:** dão uma visão local da demanda, com a ressalva de que a maioria das cidades tem poucas vendas.
- **Faturamento anual por estado e cidade:** mostra onde está a receita e como ela evoluiu ano a ano.

**O prompt e o que mudou**
- **Versão inicial:** um briefing detalhado para um HTML autônomo, com estética inspirada no site da Porsche, filtros, KPIs, gráficos, tabela e exportação, para um CSV de colunas genéricas e valores em R$.
- **Primeiro ajuste:** adaptei tudo à planilha real, que tem outros nomes de coluna, data da venda, status de entrega e valores em dólar.
- **Segundo ajuste:** acrescentei as cinco perguntas de negócio.
- **Terceiro ajuste:** retirei a leitura de arquivo (botão, arrastar e colar), e os dados passaram a ficar embutidos no HTML.
- **Quarto ajuste:** suavizei os gráficos e ajustei a fonte dos cartões, com corte de dados em 20/01/2026.
- **Versão final:** o corte passou para 14/10/2026, o alerta de registros foi removido e o hero ganhou a "Última atualização: 14/10/2026".

**Tratamento da base**
A planilha foi enviada como estava. O tratamento que fiz foi:
- **Colunas aproveitadas:** só 8 colunas entraram no dashboard, e nome de cliente e vendedor ficaram de fora.
- **Limpeza dos dados:** padronização de espaços e maiúsculas, descarte de linhas sem preço ou ano e leitura das datas, que vinham em formatos mistos.
- **Corte de período:** apenas vendas até 14/10/2026 entram, o que deixa 79 dos 100 registros.
- **Moeda:** os valores estão em dólar.

Dois pontos 19 registros têm a mesma data, 20/01/2026, que parece uma data padrão. As vendas canceladas também entram nos totais, mas dá para excluí-las pelo filtro de status de entrega.

**Recurso de IA**
O dashboard foi gerado pelo Claude (Claude Sonnet 5.5), no chat do claude.ai, que leu a planilha, escreveu o código e testou a lógica. O painel em si não usa IA ao abrir: os gráficos rodam no navegador com Plotly e o CSV exportado usa PapaParse.

<img width="1871" height="685" alt="image" src="https://github.com/user-attachments/assets/d793107f-b1dc-412a-ac3e-4c61adbd5eae" />


**Endereço publicado**
[Uploading index.html.html…]()
