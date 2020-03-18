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
- **Margem Contribuição (R$):** As 5 combinações Grupo de Cliente-GP com as  margens de contribuição (R$/ton) mais negativas.
- **P-R (R$/ton)**: As 5 combinações Grupo de Cliente-GP com os piores valores de P-R (R$/ton) mais negativos.

<img src="https://raw.githubusercontent.com/Luciano-Belgo/RGM-Guia/master/imagens/Resumo%20de%20oportunidades.png"><br>

Para analizar uma das combinações Grupo de Cliente-GP exibida no Resumo de oportunidades, clique nela com o botão direito e em **Drill-through**, escolha se você deseja analizá-la por **Dispersão**, **Cascata de Margem** ou o **P-R**. 

___
## CASCATA DE MARGEM
**Gráfico de cascata:** Clicando em "Drill-Trough" > "Cascata de Margem", você será direcionado à página com o gráfico de cascata mostrando os valores em R$/ton desde o Preço de Lista até a Margem Industrial, para que possa ser analisado quanto houve de desconto, impostos, preço do FM, etc. para o grupo de cliente e GP escolhido no Resumo de Oportunidades.

<img src="https://raw.githubusercontent.com/Luciano-Belgo/RGM-Guia/master/imagens/Cascata%20de%20margem.PNG"><br>


**Avaliação detalhada PVL:**  Na avaliação detalhada, logo abaixo do gráfico, temos duas tabelas:
- **Primeira tabela:** pode-se consultar a cascata em formato de tabela para o mês atual, assim como mostrado no gráfico de cascata. Porém nessa tabela é possível comparar os valores da cascata com períodos anteriores, utilizando o filtro de data no canto superior direito da página. Basta selecionar a data inicial e final desejada.
- **Segunda tabela:** para o mesmo período filtrado no canto superior direito da página, é possível navegar por níveis de informação mais granulares como Segmento > GP > Material > Bitola.

<img src="https://raw.githubusercontent.com/Luciano-Belgo/RGM-Guia/master/imagens/Avalia%C3%A7%C3%A3o%20detalhada.PNG"><br>

Lembrando que todas as informações exibidas na página referem-se ao grupo de cliente e GP selecionado anteriormente na página Resumo de Oportunidades. Caso queira personalizar os segmentos, clientes e GP exibidos, utilize os filtros visuais no topo da página.

**Filtros visuais:** Acima do gráfico, existem campos para filtrar o que será visualizado no gráfico de cascata e tabelas. Repare que ao clicar na caixa de seleção dos filtros "GP" e "Cliente", será exibido somente o grupo de cliente e GP selecionado na aba Resumo de Oportunidades.
Caso deseje visualizar o gráfico para outros clientes, GPs, ou períodos, clique em "Redefinir Filtros" no canto superior direito. Assim os filtros de Drill-through serão resetados e será possível filtrar o gráfico conforme desejado através dos campos de filtro. Outra opção, caso nao queira resetar todos os filtros que estão aplicados, é possível abrir a barra lateral de filtros, e na sessão "Filtros nesta página", apagar os filtros desejados (Segmento, Grupo de Cliente e/ou GP).

___
## DISPERSÃO
**Gráfico de dispersão:** Clicando em "Drill-Trough" > "Dispersão", você será direcionado à página com o gráfico de dispersão de Desconto(%) vs Volume(t). Nesse gráfico você visualizará um ponto para cada cliente do Grupo de cliente selecionado no Resumo de Oportunidades (pode ser que haja apenas um ponto), e ao lado verá o gráfico de Cascata para os pontos do gráfico de dispersão. Caso queira filtrar a cascata para apenas um dos pontos do gráfico de dispersão, basta clicar no ponto desejado e ele será realçado, filtrando assim o gráfico de cascata.

<img src="https://raw.githubusercontent.com/Luciano-Belgo/RGM-Guia/master/imagens/Dispers%C3%A3o.PNG"><br>

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

**Filtros do Drill-through:** Para comparar o grupo de cliente, cliente ou GP com outros através do gráfico de dispersão, limpe o filtro desejado na aba lateral de filtros, conforme imagem abaixo. Você pode por exemplo limpar o filtro de grupo de cliente, para comparar o volume e desconto para diferentes clientes que compraram o GP filtrado. <br><br><img src="https://github.com/Luciano-Belgo/RGM-Guia/blob/master/imagens/Limpar%20filtros%20laterais.png">

___
## P-R
**Gráfico P-R:** Clicando em "Drill-Trough" > "P-R", você será direcionado à página P-R com uma barra representando o trimestre atual, selecione no canto superior direito o período desejado para o gráfico de P-R.

**Gráficos de cascata:** Logo abaixo do P-R, pode ser visualizado um primeiro gráfico de cascata para o trimestre referência (Q4/2016) e um segundo para o período base (trimestre atual). Logo acima dos gráficos é possível alterar os períodos dos mesmos.

**Avaliação detalhada PVL:** Enquanto o gráfico exibe a cascata em um período específico, as tabelas de avaliação detalhada do PVL exibe a cascata em um intervalo de tempo selecionado.
