# Guia de uso do Relatório de Gestão de Margem (RGM)
___
## PÁGINAS DO RELATÓRIO
- Resumo de Oportunidades
- P-R
- Cascata de Margem
- Dispersão

*Acesso ao relatório:* [Power BI - RGM](https://app.powerbi.com/groups/363fc772-dd63-4b14-9874-23adbff5b394/reports/86144c27-0021-4000-8f7c-6361bf0873e2/ReportSectiond4541df725c8d50c0f4c)
___

## RESUMO DE OPORTUNIDADES
Nesta página são exibidas as 5 maiores oportunidades em cada um dos dois critérios a seguir:
- **MC Negativa:** As 5 combinações Grupo de Cliente-GP com as piores margens de contribuição (R$/ton)
- **P-R**: As 5 combinações Grupo de Cliente-GP com os piores valores de P-R (R$/ton)

Para analizar uma das combinações Grupo de Cliente-GP exibida no Resumo de oportunidades, clique nela com o botão direito e em "Drill-through", escolha se você deseja analizá-la por Dispersão, a Cascata de Margem ou o P-R. 

___
## CASCATA DE MARGEM
**Gráfico:** Clicando em "Drill-Trough" > "Cascata de Margem", você será direcionado à página com o gráfico de cascata mostrando os valores em R$/ton desde o Preço de Lista até a Margem Industrial, para que possa ser analisado quanto houve de desconto, impostos, preço do FM, etc. para o cliente e GP escolhido no Resumo de Oportunidades.

**Avaliação detalhada PVL:**  Na avaliação detalhada, logo abaixo do gráfico, pode-se consultar a cascata em formato de tabela, além do detalhamento por segmento, GP, material e bitola das vendas filtradas no gráfico.

**Filtros visuais:** Acima do gráfico, existem campos para filtrar o que será visualizado no gráfico de cascata. Repare que ao clicar na caixa de seleção dos filtros "GP" e "Cliente", será exibido somente o cliente e GP selecionado na aba Resumo de Oportunidades.
Caso deseje visualizar o gráfico para outros clientes, GPs, ou períodos, clique em "Redefinir Filtros" no canto superior direito. Assim os filtros de Drill-through serão resetados e será possível filtrar o gráfico conforme desejado através dos campos de filtro.

___
## DISPERSÃO
**Gráfico:** Clicando em "Drill-Trough" > "Dispersão", você será direcionado à página com o gráfico de dispersão de Desconto(%) vs Volume(t). Nesse gráfico você visualizará um ponto para cada cliente do Grupo de cliente selecionado no Resumo de Oportunidades (pode ser que haja apenas um ponto), e ao lado verá o gráfico de Cascata para os pontos do gráfico de dispersão. Caso queira filtrar a cascata para apenas um dos pontos do gráfico de dispersão, basta clicar no ponto desejado e ele será realçado, filtrando assim o gráfico de cascata.

**Drill-down:** O Power BI fornece uma ferramenta muito poderosa de navegação interativa entre hierarquias dos visuais, conhecida como Drill-down. Apesar de parecer um pouco confuso no início, ao dominar essa ferramenta de navegação o usuário terá um poder de análise bem mais detalhada em suas mãos.
O gráfico de dispersão permite esse tipo de navegação, pois possui a seguinte estrutura hierarquica: "Grupo de Cliente", "Cliente" e "Nº de documento", ou seja, podemos utilizar o gráfico de três formas diferentes. 
- A primeira forma é onde cada ponto do gráfico representa um grupo de cliente.
- A segunda forma é onde cada ponto do gráfico representa um cliente.
- A terceira forma, no maior nível de granularidade, podemos ver cada ponto como um Nº de documento (OV). 

Podemos por exemplo querer visualizar o gráfico com cada ponto sendo um cliente dentro de um segmento, e então decidimos visualizar as ordens de venda de um determinado cliente que encontramos no gráfico. Essa navegação entre grupo de clientes, clientes e OVs é feita a através dos botões de navegação de Drill-Down e Drill-Up encontrados no topo do gráfico, conforme imagem abaixo:<br><br>
<img src="https://github.com/Luciano-Belgo/RGM-Guia/blob/master/drill%20down%20-%20drill%20up.png"><br>

- A **terceira seta**, representada com o número 3 na imagem acima, avança para o próximo nível de hierarquia. Se você estiver visualizando os grupos de clientes no gráfico, ao clicar na terceira seta você passará a ver cada ponto como um cliente, e se clicar novamente você chegará ao nivel de maior granilaridade, onde cada ponto do gráfico representa uma OV.

- Já a **primeira seta** faz o chamado Drill up, ou seja, o caminho inverso da terceira seta, subindo a hierarquia de OV para cliente e de cliente para grupo de cliente.

- A **segunda seta** é o reucrso que habilita o Drill Down. Clicando nessa seta, ela ficará com um circulo preto, enquanto ela tiver habilitada, você poderá clicar em algum gurpo de cliente para visualizar todos os clientes daquele grupo. Caso habilite o Drill-Down na hierarquia de clientes, você poderá clicar em um cliente para visualizar todas as OVs apenas daquele cliente selecionado. Observe que para poder filtrar algum ponto no gráfico é necessário desabilitar a seta de Drill-Down.

**Filtros visuais:** Acima do gráfico, asism como na página "Cascata", existem campos para filtrar o que será visualizado nos gráficos abaixo. Repare que ao clicar na caixa de seleção dos filtros "Grupo Cliente", "Cliente" e "GP", será exibido somente o grupo de cliente, cliente e GP selecionado na aba Resumo de Oportunidades. Isso ocorre pois a visualização está filtrada pelo Drill-Through da página "Resumo de oportunidades". Caso deseje visualizar o gráfico para outros clientes, GPs, ou períodos, clique em "Redefinir Filtros" no canto superior direito. Assim os filtros de Drill-through serão resetados e será possível filtrar o gráfico conforme desejado através dos campos de filtro.

**Filtros do Drill-through:** Para comparar o grupo de cliente, cliente ou GP com outros através do gráfico de dispersão, limpe o filtro desejado na aba lateral de filtros, conforme imagem abaixo:<br><br><img src="https://github.com/Luciano-Belgo/RGM-Guia/blob/master/imagens/Limpar%20filtros%20laterais.png">
