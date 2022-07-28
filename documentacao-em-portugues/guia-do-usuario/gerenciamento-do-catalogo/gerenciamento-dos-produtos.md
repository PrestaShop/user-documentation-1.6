# Gerenciamento dos Produtos

Você pode gerenciar seus produtos na sua loja com a página "Produtos", no menu "Catálogo ".

Seções neste capítulo:

* [A Lista de Produtos](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-AListadeProdutos)
* [Os Botões Globais da Página de Criação do Produto](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-OsBotõesGlobaisdaPáginadeCriaçãodoProduto)
* [Preenchendo as informações do Produto](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-PreenchendoasinformaçõesdoProduto)
* [Escolhendo o Preço de um Produto](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-EscolhendooPreçodeumProduto)
* [Preços específicos: Gerenciando a Quantidade de Discontos](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-Preçosespecíficos:GerenciandoaQuantidadedeDiscontos)
* [Gerenciamento da Prioridade do Preço](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-GerenciamentodaPrioridadedoPreço)
* [Otimizando a posição do seu produto no motor de busca (SEO)](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-Otimizandoaposiçãodoseuprodutonomotordebusca\(SEO\))
* [Gerenciamento das Associações do Produto  ](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-GerenciamentodasAssociaçõesdoProduto)
* [Categorias de produto](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-Categoriasdeproduto)
* [Acessórios](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-Acessórios)
* [Fabricante](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-Fabricante)
* [Adicionando Combinações de Produtos](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-AdicionandoCombinaçõesdeProdutos)
* [Método manual](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-Métodomanual)
* [Método Automático](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-MétodoAutomático)
* [Gerenciamento da Quantidades dos Produtos](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-GerenciamentodaQuantidadesdosProdutos)
* [ Gerenciamento dos anexos](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-Gerenciamentodosanexos)
* [ Configuração do Fornecedor do Produto](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-ConfiguraçãodoFornecedordoProduto)
* [ Gerenciamento de Estoques (avançado)](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-GerenciamentodeEstoques\(avançado\))

[ Criando um Pacote de Produtos](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-CriandoumPacotedeProdutos)

* [ Quantidades do kit](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-Quantidadesdokit)

[ Criando um Produto Virtual](gerenciamento-dos-produtos.md#GerenciamentodosProdutos-CriandoumProdutoVirtual)

### A Lista de Produtos <a href="#gerenciamentodosprodutos-alistadeprodutos" id="gerenciamentodosprodutos-alistadeprodutos"></a>

Clicar na opção "Produtos" do menu "Catálogo" é redireciona você para a lista dos seus produtos, exibidos com suas principais informações: ID, foto, nome, referência, categoria, etc.

\- Imagem -

Além da lista de produtos, esta página apresenta para você quatro estatísticas da sua loja:

* Percentual de itens em estoque
* Percentual da margem bruta da média
* Percentual das vendas durante os últimos 30 dias
* Número de produtos desativados.

A opção "Filtro por categoria" deixa você ver apenas os produtos pertencentes a sua pesquisa atual, como também reorganizar a posição dos produtos em uma categoria.

Posição do produto

Você não pode reorganizar toda a lista de produtos. Os produtos são exibidos como em sua vitrine (aumentando o número do ID), e o cliente pode escolher a ordem dos produtos com as seguintes opções: preço mais baixo primeiro, nome do produto de A a Z nome do produto de Z a A, primeiro em estoque, menor referência primeiro, maior referência primeiro.

Você pode organizar produtos de acordo com a categoria marcando a opção "Filtrar por categoria". Isto abrirá uma interface listando todas as suas categorias e subcategorias. Selecionar uma categoria faz com que seja filtrado na lista de produtos apenas produtos da categoria selecionada. Também adiciona uma coluna chamada "Posição" á tabela, com a qual você pode ordenar o produto na página da categoria. Isto é feito ou movendo os produtos para cima ou para baixo, ou clicando nas setas.

A ordem do seu produto pode ser alterada pela escolha de ordenação do usuário.

Note que quando você muda a ordem de exibição na lista de produtos no back office (clicando nas setas nos nomes das colunas para ordenar os produtos de acordo com a coluna), a coluna "Posição" não mostra essas setas e você também não pode usa-las para mover os produtos. Ao contrário, mostra o número da posição do produto. Para poder posicionar os produtos novamente clique no botão "Resetar".

Finalmente, o topo da lista de produto apresenta cinco botões:

\- Imagem -

* **Adicionar novo produto**. Cria um novo produto.
* **Exportar**. Baixa um arquivo CSV de todos os produtos no seu catálogo.
* **Importar**. Redireciona você para a página de Importação de CSV, na qual você pode importar seus arquivos CSV.
* **Atualizar Lista**. Recarrega a lista de produtos para mostrar as últimas alterações.
* **SQL**. Proporciona uma query em SQL para reproduzir sua pesquisa de produtos ou filtrar no seu próprio gerenciador de SQL.
* **Exportar para o Gerenciador de SQL**. Abre o menu da ferramenta Gerenciador de SQL da PrestaShop (localizada em "Parâmetros Avançados"), de onde você pode consultar, alterar, inserir e excluir dados do banco de dados da sua loja PrestaShop com SQLs ("`SELECT ... FROM ... WHERE ...`"). Se sua lista de produtos foi filtrada (pelo nome, por exemplo), então a SQL padrão será utilizada (por exemplo, "``WHERE 1  AND b.`name` LIKE '%blouse%'``").

Você pode adicionar novos produtos clicando em "Adicionar novo". Uma janela aparecerá, com várias abas na coluna á esquerda e dois botões no topo: "Voltar á lista" e "Ajuda".

### Os Botões Globais da Página de Criação do Produto <a href="#gerenciamentodosprodutos-osbotoesglobaisdapaginadecriacaodoproduto" id="gerenciamentodosprodutos-osbotoesglobaisdapaginadecriacaodoproduto"></a>

Por padrão, a página de criação de produto tem dois botões que você encontrará em quase todas as páginas administrativa: " Módulos e Serviços Recomendados" e "Ajuda".

No rodapé de cada página, existem três botões:

* **Salvar**. Este botão salva qualquer alteração que você tenha feito no produto atual/ selecionado, e redireciona você para a lista de produtos.
* **Salvar e Continuar**. Este botão salva qualquer alteração que você tenha feito no produto atual/ selecionado e mantem você na mesma aba. Isto é útil quando você quer ir para outra aba sem perder as alterações na aba atual, ou para ver suas alterações serem aplicadas imediatamente.
* **Cancelar**. Este botão simplesmente te redireciona para a lista de produtos, sem salvar nenhuma das alterações que você fez em qualquer aba desta página.

\- Imagem -

Assim que você der um nome ao seu novo produto e clicar no botão "Salvar e continuar" no rodapé, mais botões aparecerão no topo da sua página de produto:

* Pré-visualização. Mostra a página da vitrine do seu produto. Isto é muito conveniente, já que funciona mesmo se o produto estiver desativado (aba "Informação").
* Duplicar. Cria uma cópia exata do produto selecionado. Isto é muito útil quando você prefere utilizar os dados do produto atual como modelo para outro novo produto, e não ter que criar todos os dados do novo produto à mão. Por exemplo, dois produtos podem ser muito diferentes, mas podem compartilhar as mesmas associações, transportadoras ou configuração se fornecedores.

Não exagere nas duplicações!

Se você precisar criar versões diferentes do mesmo produto, por causa da sua variedade de cores, capacidade, tamanho, etc., então você deveria criar combinação de produto para o produto atual ao invés de duplica-lo X vezes. Veja a aba "Combinações" à esquerda, a qual é explicada na seção "Adicionando Combinações de Produto" deste capítulo.

* **Vendas do produto**. Redireciona você para a página "Detalhe do produto" do painel de estatísticas (Menu "Stats"), o qual dá a você um gráfico de ambas as visitas para esta página do produto, e também as suas vendas.
* **Deletar este produto**. Remove todos os dados do produto atual, incluindo suas imagens, combinações, características, etc.
* **Módulos recomendados**. Abre uma nova janela sugerindo você a instalar alguns módulos populares da loja de Extensões PrestaShop.

\- Imagem -

### Preenchendo as informações do Produto <a href="#gerenciamentodosprodutos-preenchendoasinformacoesdoproduto" id="gerenciamentodosprodutos-preenchendoasinformacoesdoproduto"></a>

A primeira aba contém a informação básica sobre o produto.

\- Imagem -

A primeira linha é essencial: indica se o produto é um kit (uma combinação de pelo menos dois produtos existentes), um produto virtual (arquivo para baixar, serviço, etc.), ou um simples e clássico, produto enviado fisicamente. Por de enquanto, nós apenas explorarem os o produto clássico, e lidaremos com produtos kit e virtual nas suas próprias seções deste capítulo.

Existem mais opções relacionadas a produtos na página "Produtos" do menu "Preferências":

* Número de dias pelo qual o produto é considerado 'novo'.
* Ordenação padrão do produto.
* Habilitar gerenciamento avançado de estoque.
* etc.

Você realmente deveria conferir que essas configurações estão configuradas como você deseja.

Você começa com quatro campos:

* **Nome**. O primeiro campo a ser preenchido é o nome do produto, que aparecerá nos resultados do motor de busca. Próximo ao campo você encontrará o código do idioma, que habilita você a escolher o idioma no qual você deseja editar ou criar o nome.

Você deve dar ao produto um nome pelo menor no idioma padrão antes de você salva-lo. Você não poderá salva-lo até que ele tenha um nome - e muitas outras abas exigem que o produto esteja salvo para poderem ser acessadas.

Tenha certeza de traduzir cada campo em todos os idiomas que sua loja suporta. Para fazer isso, clique no código do idioma próximo do campo, e escolha o idioma no qual você deseja editar o texto.

* **Código de referência**. Esta é a referência do seu produto em sua loja. Pose ser um número, o a referência dele em um lugar no estoque ou do fornecedor, or qualquer coisa que o faça único.
* **Código de barras EAN-13 ou JAN**. Estes são os números do código de barras do produto, que são mundialmente utilizados para identifica-lo. Você pode utilizar um código do tipo EAN-13 ou JAN.
  * Um código de barras do tipo EAN-13 é o código internacional de 13 dígitos do produto. Leia mais na Wikipedia: [https://pt.wikipedia.org/wiki/EAN-13](https://pt.wikipedia.org/wiki/EAN-13)
  * Um código de barras do tipo JAN é específico do Japão, mas é compatível com o EAN internacional. Leia mais na Wikipedia: [https://en.wikipedia.org/wiki/International\_Article\_Number#jan](https://en.wikipedia.org/wiki/International\_Article\_Number#jan).
* **UPC**. Um código de barras, mais utilizado na América do Norte, Reino Unido, Austrália e Nova Zelândia. Leia mais na Wikipedia: [https://en.wikipedia.org/wiki/Universal\_Product\_Code](https://en.wikipedia.org/wiki/Universal\_Product\_Code)

Então vem quatro opções:

* **Habilitado**. Se você não quiser que este produto fique imediatamente visível ou disponível para seus clientes, altere esta opção para "Não".
* **Visibilidade**. Você pode escolher quais canais você deseja disponibilizar o produto.
  * **Todo lugar**. Clientes podem chegar ao produto explorando o catálogo, na procura pelo nome do produto, ou diretamente pela URL.
  * **Catálogo**. Clientes podem chegar ao produto procurando no catálogo ou diretamente pela URL.
  * **Procura**. Clientes podem chegar ao produto procurando pelo nome ou diretamente pela URL.
  * **Nenhum lugar**. Clientes podem chegar ao produto apenas através da URL. Eles não encontrarão o produto procurando pelo catálogo  ou procurando pelo nome. Esta opção é ótima para a criação de produtos particulares, para que apenas visitantes confiados possam acessar, mesmo temporariamente (você pode alterar esta configuração a qualquer momento).
* **Opções**. Algumas opções especificas.
  * **Disponível para venda**. Se você desmarcar essa opção, os clientes não poderão adicionar esse produto carrinho. Isto faz com que o catálogo fique em um modo parecido com produto único (em comparação com a configuração "modo Catálogo").
  * **Mostrar preço**. Mesmo se a opção "disponível para venda" estiver desmarcada, você poderá escolher mostrar o preço ou não (mesmo que os visitantes não possam compra-los).
  * **Apenas online (não vendido em loja física)**. Se o seu negócio tiver lojas físicas, esta opção não terá valor quando um produto for vendido apenas online, não fisicamente, isto previne clientes de conferir o preço do produto onli e, e então vir a sua loja esperando compra-lo diretamente para evitar o preço de envio.
* **Condição**. Nem todas as lojas vendem produtos novos. Esta opção permite que você indique a condição do produto:
  * **Novo**. O produto é novo, lacrado no pacote original.
  * **Usado**. O produto foi vendido pelo menos uma vez antes, e provavelmente usado por alguém (segunda mão). Deveria vir no pacote original, que pode está fechado com fita adesiva.
  * **Renovado (refurbished)**. O produto foi retornado por várias razões ("arranhados, amassados ou outros defeitos cosméticos que não afetam a performance do produto"). Leia mais na Wikipedia: [https://pt.wikipedia.org/wiki/Restauração\_(processo)](https://pt.wikipedia.org/wiki/Restaura%C3%A7%C3%A3o\_\(processo\))

Agora que todos estes detalhes foram explicados, você pode começar adicionando uma descrição ao seu produto.

Descrever seu produto bem é essencial, para ambos o cliente (quanto mais informação melhor) e para motores de busca (ajudara sua loja a aparecer em mais pesquisas).

\- Imagem -

No rodapé da tela, cada campo dos dois campos de descrição tem diferentes propósitos:

* O **campo "Descrição curta"** habilita você a escrever uma descrição curta que aparecerá em motores de busca e na descrição da categoria do seu produto. Este campo é limitado á 400 caracteres por padrão: se você exceder este limite, PrestaShop te avisara com uma mensagem em vermelho abaixo do campo. Você pose mudar este limite na página preferências dos "Produtos", na qual você encontrará a opção " Tamanho máximo da descrição curta".
* O **campo "Descrição"** habilita você a escrever uma descrição completa do seu produto, que aparecerá diretamente na página do produto. O editor de texto oferece uma gama de opções para criar descrições visualmente atrativas (fonte, tamanho, cor do texto, etc.). Enquanto o segundo campo não tem limites, existem algo como muito conteúdo: esforce-se para informar o essencial de uma maneira atrativa, e seu produto estará pronto para ser vendido.

Abaixo do campo "Descrição", você pode encontrar uma pequena ferramenta para adicionar uma das imagens que você anexou ao produto (através da aba "Imagens") a "Descrição", usando tags de imagem. Clique em "Clique aqui" para abri-la.

\- Imagem -

Simplesmente selecione a imagem que você quer, escolha a posição de acordo como o texto e o tamanho, e PrestaShop gerará uma tag de imagem que você poderá colocar na descrição (preferivelmente entre dois parágrafos, ou no começo de um parágrafo).

No **campo "Tags"**, adicione alguns termos e palavras chave que ajudarão seus clientes a encontrar facilmente o que eles estão procurando.

\- Imagem -

Elas são exibidas na loja no bloco "Tags" (se disponível). Se você não quer que o bloco tag seja exibido, simplesmente desative o módulo "Bloco de tags" (na página "Módulos").

Diferenças com PrestaShop 1.4

PrestaShop 1.4 permite a você indicar o fabricante do produto nessa aba. Desde a versão 1.5 esta configuração está na aba "Associações" á esquerda. Mesma coisa para o campo "Categoria padrão", as categorias associadas, e o campo " Acessório".

A versão 1.4 também permite você indicar o tamanho e peso do pacote final. Desda versão 1.5, estas configurações são encontradas na aba "Envio" à esquerda.

O campo "Locação" da versão 1.4 pode ser encontrado na aba opcional á esquerda "Armazéns", que é disponível apenas quando habilitado a Administração Avançada de Estoque (menu "Preferências", página "Produtos", seção "Estoque de produtos").

Assim que você tiver preenchido todas estas informações, salve seu trabalho, que depois será enviado a sua lista de produtos. Se você salvar clicando em " Salvar e Continuar", você poderá continuar trabalhando na apresentação das informações do seu produto.

### Escolhendo o Preço de um Produto <a href="#gerenciamentodosprodutos-escolhendooprecodeumproduto" id="gerenciamentodosprodutos-escolhendooprecodeumproduto"></a>

Tudo isto é feito na aba "Preços" à esquerda. A seção de preço pode ser bem intimidante, com campos influenciando uns aos outros e taxas a serem consideradas - mas na verdade é bem simples.

\- Imagem -

Escolha o preço que aparecerá na sua loja seguindo as instruções abaixo:

* **Preço por atacado**. Permite você a instantaneamente saber seu preço por atacado, preço de fábrica, e portanto comparar com seu preço de venda para facilmente calcular seu lucro.
* **Preço de varejo**. O preço do seu lucro produto antes das taxas.
* **Regra tributária**. O imposto aplicável ao produto. Escolha entre diferentes taxas que você tem registradas.\
  Se você precisa criar novas taxas de impostos, clique no botão "Criar Novo Imposto". A criação do imposto é feita no menu "Localização", página "Impostos"; essa parte é completamente explicada no capítulo "Entendendo as Configurações Locais" deste guia.
* **Ecotaxa (imposto incluído)**. O valor da ecotaxa para este produto. Este valor já está incluído no seu preço de varajo. Você supostamente tem que declarar este imposto a agência de impostos de seu país.\
  _Perceba que esse campo não mostrado por padrão_. Se você tiver que incluir uma ecotaxa, primeiro você deve habilita-la: vá para o menu "Localização", página "Impostos", seção "Opções de impostos" (rodapé da página), e escolha "Sim" para a opção "Usar ecotaxa".
* **Preço de varejo com imposto**. Mostra o preço do produto com impostos incluídos. Você pode editar o valor, e isso automaticamente atualizará o campo "Preço de varejo antes do imposto" de acordo com a regra de imposto que você escolheu.
* **Preço unitário**. Permite a você mostrar o preço unitário conforme a legislação local. Por exemplo, se você está vendendo um pacotes se 6 latas de um refrigerante, então você deve preencher este campo com seu preço por lata, e indicar "lata" no campo de texto. A descrição na mesma linha atualizará de acordo.
* **Mostra o ícone "a venda" na página do produto e no texto encontrado na listagem do produto**. Marque está opção para mostrar que seu produto está a venda, tanto na página do produto quanto no texto da listagem do produto. Um ícone "A venda" aparecerá abaixo do produto. Você pode modificar esta frase alterando o seguinte arquivo: themes/default/img/onsale\_br.gif
* **Preço final de varejo**. Este preço, incluindo o desconto considerado, serão atualizados conforme você digita.

Você pode preencher o campo "preço de varejo com imposto" e escolher a taxa de imposto a ser aplicada, e o campo calculará automaticamente o preço de varejo antes do imposto. A operação oposta também está disponível.

Neste ponto, você terminou com as informações essenciais para uma página de produto básica. Você pode salvar e te-lo imediatamente disponível para venda vender em sua loja!\
Mas continue lendo, já que existem muito mais detalhes que você pode adicionar para o seu produto para torna-lo mais atrativo para seus clientes.

### Preços específicos: Gerenciando a Quantidade de Discontos <a href="#gerenciamentodosprodutos-precosespecificos-gerenciandoaquantidadedediscontos" id="gerenciamentodosprodutos-precosespecificos-gerenciandoaquantidadedediscontos"></a>

Você pode mudar o preço total do produto dependendo da quantidade do produto que seu cliente compra, o grupo do usuário, o país, etc. Isto é feito na seção "Preços específicos" da aba "Preços". Clique no botão "Criar um novo preço específico" para mostrar a janela de criação.

\- Imagem -

Esta é uma maneira muito fácil de criar um preço de desconto para este produto (e todas as suas combinações).

Clique em "Adicionar um Novo preço específico", e um formulário aparecerá.

* **Para**. Esta opção permite que você seja bem específico sobre os vários grupos aos quais o preço se aplica, incluindo moedas, países e até grupos de clientes (o qual discutirem os mais tarde neste capítulo).
* **Cliente**. Você pode escolher ser mais específico ainda e configurar diretamente a quem o desconto que você está criando é direcionado. Comece digitando as primeiras letras do primeiro ou segundo nome do cliente que você quer.
* **Combinação**. Você pode escolher aplicar este preço em específico para todas as combinações, ou apenas uma. Se você deseja aplicar a mais de uma combinação mas não todas elas, você terá que criar um preço especifico para cada combinação.
* **Disponível de/para**. Aqui você pode definir um intervalo de datas entre as quais o preço de desconto está ativo. Clicando em cada seletor abrira um calendário, simplificando o processo.
* **Começando na unidade \[]**. Contém o valor do qual o desconto deveria ser aplicado. O padrão é "1", que significa qualquer quantidade.
* **Preço do produto (sem imposto)**. Aqui é onde você pode configurar um preço arbitrário, independente dos cálculos e preços regulares. Mantenha este campo igual a "0" para usar o preço padrão.
* **Manter o preço básico**. Marque esta opção para resetar o campo "Preço do produto" e previnir você mesmo de editar isto.
* **Aplique um desconto**. O desconto que será aplicado uma vez que o cliente escolheu a quantidade do produto. Use o seletor para escolher o tipo do descontos (tanto uma quantidade específica na moeda padrão, ou um percentual do preço padrão).

Uma vez que você tenha seus valores clique em "Salvar e continuar": o sumário das configurações do seu desconto aparecem abaixo.

O desconto será imediatamente visível na loja.

Se você desejá deletar um valor, clique no ícone da lixeira na tabela.

Se você quiser criar descontos mais complexos, leia sobre o menu "Regras de preço" no capítulo "Criando Regras de Preços e comprovantes" deste guia.

### Gerenciamento da Prioridade do Preço <a href="#gerenciamentodosprodutos-gerenciamentodaprioridadedopreco" id="gerenciamentodosprodutos-gerenciamentodaprioridadedopreco"></a>

Um cliente pode se encaixar em múltiplas regras e preços ou descontos, até mesmo quando você detalhou preços e descontos, com grupos customizados e lojas (se estiver em um contexto multi loja). PrestaShop antes de tudo usa um conjunto de prioridades em ordem para aplicar uma regra em particular para tais clientes. Você pode querer que o grupo de usuário tenha mais importância do que a moeda, por exemplo.

Você pode trocar as configurações padrão do PrestaShop usando a seção "Gerenciamento de Prioridades".

\- Imagem -

A ordem padrão de importância é:

1. Loja (quando em um contexto multi loja).
2. Moeda.
3. País.
4. Grupo.

Uma opção no rodapé habilita você a atualizar as configurações de todos os produtos. Se a opção permanecer desmarcada, então suas alterações aplicam apenas ao produto atual.

### Otimizando a posição do seu produto no motor de busca (SEO) <a href="#gerenciamentodosprodutos-otimizandoaposicaodoseuprodutonomotordebusca-seo" id="gerenciamentodosprodutos-otimizandoaposicaodoseuprodutonomotordebusca-seo"></a>

Para melhorar a listagem do seu produto tão quanto aumentar a visibilidade da sua loja nós sugerimos que você cuidadosamente preencha todos os campos SEO: meta titles, meta description, e keywords e URLs amigáveis.

"SEO" por si só significa "Otimização para motores de busca". Leia mais na Wikipedia: [pt.wikipedia.org/wiki/Otimização\_para\_motores\_de\_busca](http://pt.wikipedia.org/wiki/Otimiza%C3%A7%C3%A3o\_para\_motores\_de\_busca)

[Saiba quais são as melhores práticas de SEO para e-commerce! Baixe e leia o "Guia Completo para SEO" da PrestaShop gratuitamente: ](http://pt.wikipedia.org/wiki/Otimiza%C3%A7%C3%A3o\_para\_motores\_de\_busca)[http://www.prestashol.com/en/white-paper-seo](http://www.prestashol.com/en/white-paper-seo)

Para acessar as informações SEO do produto, abra a aba "SEO" á esquerda.\
&#x20;

\- Imagem -

Os campos nesta página habilitam você a otimizar diretamente a visibilidade do seu catálogo em moters de busca.

* **Meta title**. Este é o campo mais importante, já que o título aparecerá  todos os motores de busca. Seja bem factual: você deve convencer o usuário do motor de busca a clicar no seu link, não noutro de outro site. Tenha certeza que o título é único para esse produto. Um bom exemplo: "Calça Jeans Levi's 501® Original Jeans Tidal Blue - Original Fit". Mal exemplo: " Item #02769869B bestseller".
* **Meta description**. Uma representação do produto em apenas algumas linhas (idealmente, menos que 155 caracteres), feita para capturar o interesse do cliente. Isto aparecerá nos resultados para alguns motores de busca, dependendo dos argumentos da busca: alguns motores de busca podem escolher exibir as palavras chaves diretamente no contexto do conteúdo da página. Tenha certeza de que este produto esteja no seu site.
* **URL amigável**. Este é outro campo extremamente importante. Habilita você a reescrever o endereço do seu produto como você desejar. Por exemplo, ao invés de ter um endereço como\
  [http://www.myprestashop.prestashop.com/index.php?id\_product=8\&controller=product](http://www.myprestashop.prestashop.com/index.php?id\_product=8\&controller=product)\
  você pode ter:\
  [http://www.myprestashop.prestashop.com/8-nome-do-produto.html](http://www.myprestashop.prestashop.com/8-nome-do-produto.html).\
  Tudo que você precisa fazer é indicar no campo "URL amigável" as palavras que você deseja que apareçam ao invés do nome padrão, separado por hífens.\
  O botão "**Gerar**" facilita a criação apropriada de uma URL amigável baseado no nome do produto. Uma vez gerado, você pode editar editar a URL produzida se necessário.

URLs amigáveis funcionarão apenas se a reescritura de URL estiver habilitada. Você pode fazer isso na página de configuração "SEO & URLs", na seção " Configurar URLs".

Você encontrará mais informações na página de configuração "SEO & URLs" no capítulo "Entendendo as Configurações" deste guia.

### Gerenciamento das Associações do Produto   <a href="#gerenciamentodosprodutos-gerenciamentodasassociacoesdoproduto" id="gerenciamentodosprodutos-gerenciamentodasassociacoesdoproduto"></a>

Criar associações para seu produto significa atrela-lo a outros conteúdos no seu banco de dados:

* Categorias de produto.
* Outros produtos (acessórios).
* Fabricante.

\- Imagem -

### Categorias de produto <a href="#gerenciamentodosprodutos-categoriasdeproduto" id="gerenciamentodosprodutos-categoriasdeproduto"></a>

A seção "Categorias associadas" permite que você selecione em qual categoria o produto deveria aparecer. Você pode selecionar mais de uma, mas tenha em mente que é melhor para o cliente se a categoria conter apenas produtos semelhantes. Portanto, você deveria evitar selecionar categorias raiz, e preferir subcategorias.\
Por exemplo, a categoria "telefone" pode ter as subcategorias "marcas" (Apple, Samsung, Nokia, etc.) como também "características" (smartphone, abre e fecha, etc.). É de sua responsabilidade indicar as categorias mais úteis para os seus clientes.\
Se você sentir que você precisa adicionar uma categoria, salve o estado atual do seu produto antes de clicar no botão "Criar nova categoria". A criação de categoria é explicada em outra seção deste guia.\
O seletor da "Categoria padrão" é útil quando um artigo é colocado em diversas categorias. Ele serve principalmente para esclarecer qual categoria utilizar caso seu cliente chegue ao seu site a partir de um motor de busca, já que o nome da categoria aparecerá na URL do produto.

Lista de Destaque

Marcando a opção "Home" permite que você  destaque seu produto na página inicial da sua loja, desde que seu tema ofereça suporte para isso. Para remover um produto da Lista de destaque, simplesmente desmarque a opção "Home".

### Acessórios   <a href="#gerenciamentodosprodutos-acessorios" id="gerenciamentodosprodutos-acessorios"></a>

O campo "Acessórios" te dá a opção de escolher produtos relevantes para associa-los com este produto, pada sugeri-los ao seu cliente quando ele visitar a página do produto (se o tema oferecer suporte para isso). Digite as primeiras letras do nome do produto e selecione-o. O produto então será adicionado no rodapé do campo.

\- Imagem -\
&#x20;

Você pode associar um produto com quantos outros produtos conforme você achar necessário. Clique na cruz para deletar a associação do produto.

Uma associação vai apenas em uma direção: o produto associado não terá uma associação com o produto atual nesta página de configuração.&#x20;

A adição/remoção de acessórios não é automaticamente salvo! Não esqueça de clicar no botão "Salvar".

### Fabricante <a href="#gerenciamentodosprodutos-fabricante" id="gerenciamentodosprodutos-fabricante"></a>

&#x20;Um produto pode ser associado apenas com um fabricante. Escolha um na lista ou crie novo fabricante de necessário (mas salve seu produto atual clicando no link "Criando um novo fabricante").

&#x20;Medindo o Custo de Envio: Tamanho, Peso, Transportadora

&#x20;Custos de envio não devem ser negligenciados: eles podem facilmente dobrar o custo final de um pedido, e você deveria ser muito cuidadoso com eles - clientes odeiam más surpresas.

&#x20;\- Imagem -

&#x20;A aba "Envio" á esquerda permite você dar alguns detalhes preciosos sobre o pacote do seu produto:

* **Largura, altura, profundidade e peso do pacote**. Você deve se esforçar para preencher cada campo, porque sabendo o tamanho e o peso exato do seu pacote não é apenas útil para você, mas o PrestaShop pode também direcionar tamanhos/pesos específicos para transportadoras específicas automaticamente, baseado nessas configurações. O preço final do seu pedido aparecerá assim que o PrestaShop (ou o cliente) tiver selecionado uma transportadora.

Estes valores usam o peso padrão, volume, distância e unidades de dimensão, como configurado na página "Localização" no menu "Localização".

Estes valores não precisam ser inteiros. Se o peso dos seus produtos forem menores que 1 kg, você pode simplesmente usar uma virgula para indicar frações:

* 15 kgs
* 1,5 kgs
* 0,15kgs (igual a 150 g)
* et
* **Taxas adicionais de envio**. Isto pode provar ser muito útil para produtos específicos que são particularmente difíceis para empacotar, ou muito pesados.
* **Transportadoras**. Você pode escolher ter o produto atual apenas para ser enviado por um conjunto de transportadoras. Se nenhuma transportadora for selecionada então todas as transportadoras estarão disponíveis para os pedidos do cliente.

### Adicionando Combinações de Produtos <a href="#gerenciamentodosprodutos-adicionandocombinacoesdeprodutos" id="gerenciamentodosprodutos-adicionandocombinacoesdeprodutos"></a>

Você frequentemente venderá o mesmo produto sob diferentes versões: eles compartilham nomes parecidos, mas eles podem ter cores diferentes, capacidade, tamanho de tela, e outros atributos. Geralmente, estes atributos vem juntos: você poderia ter uma versão vermelha do produto tanto com capacidade de 1 GB e de 2 GB, ou com uma tela de 12" ou 15" polegadas. Por causa disso a PrestaShop chama essas versões de "combinações": seu estoque de produtos pode ser composto de várias variações de apenas um produto, o que na prática são simplesmente seus atributos combinados de maneiras específicas.

Você não pode criar combinações se você não tiver configurado corretamente os atributos dos produtos no PrestaShop.

Também, você não pode criar combinações para características que seus clientes não deveriam escolher.

A criação dos atributos é feita na página "Atributos de Produto" no menu "Catálogo, e é explicada em detalhes no capítulo do mesmo nome neste guia.

&#x20;\- Imagem -

Como seus atributos de produto são combinados é escolha sua, e a PrestaShop dá a você dois métodos para conseguir isso.

### Método manual <a href="#gerenciamentodosprodutos-metodomanual" id="gerenciamentodosprodutos-metodomanual"></a>

Este método ajuda você a criar combinações uma depois da outra. Portanto, é reservado para produtos com poucas combinações, ou produtos com combinações muito específicas que não podem ser criadas confiavelmente usando o método automático (veja a próxima seção).

\- Imagem -

Adicionar uma nova variação para seu produto leva apenas algumas etapas. Clique no botão "Nova Combinação" no rodapé da página, próximo dos botões "Salvar". Um formulário aparecerá:

* **Par atributo-valor**.

1. A partir do menu-lista, escolha um grupo de atributo, tal como "Cor" por exemplo. O conteúdo da lista "Valor" atualiza de acordo.
2. Escolha o valor do atributo que você gostaria de incluir, por exemplo "Azul".
3. Clique no botão "Adicionar" e isso aparecerá no seletor.\
   Você pode adicionar quantos pares atributo-valor forem necessários para uma combinação.\
   Você pode adicionar apenas um par por atributo para uma combinação: é impossível ter ambos "Cor: Azul" e "Cor Vermelha" nos seus pares; se isso for necessário, você terá que criar novos atributos, por exemplo "Cor primária" e "Cor secundária".\
   Você pode excluir um par atributo-valor selecionando-o e clicando no botão "Excluir".

* **Referência, EAN-13 &  UPC**. Se necessário, indique a referência da combinação, números EAN-13 e/ou UPC em cada campo, como se você estivesse criando um produto na PrestaShop. Estes números podem ser utilizados pelo seu armazém ou sua transportadora, então tenha certeza de preencher todos estes campos, eles são geralmente essenciais para o seu negócio.
* **Preço por atacado**. Este campo é útil se o preço original do produto mude simplesmente porque esta é uma combinação.
* **Impacto no preço unitário/peso/preço**. Se a combinação supostamente tem que ter um impacto no preço/peso/preço unitário original do produto, escolha a lista apropriada, selecione "Aumentar" ou "Reduzir" dependendo do contexto, e preencha o campo que aparece com o valor desse impacto.
* **Ecotaxa**. A ecotaxa específica para esta combinação (se a opção ecotaxa estiver habilitada).
* **Quantidade mínima**. Você pode preferir que esta combinação seja vendida apenas em pacotes. Use este campo para indicar o número de itens a formar esse pacote.
* **Data disponível**. Se este produto não tem no estoque, você pode indicar quando o produto estará disponível novamente.
* **Imagem**. As imagens que são relacionadas ao produto original (enviadas pelo formulário na aba "Imagens" à esquerda) serão exibidas. Marque a imagem que melhor representa esta combinação.
* **Padrão**. Marque esta opção se você quiser que a combinação que você está criando seja a principal para este produto.

Quando você tiver todos os detalhes da combinação, salve as alterações no seu produto usando o botão "Salvar e continuar". Sua combinação aparecerá na lista de atributos no rodapé da tela.

Diferenças com o PrestaSop 1.4

No PrestaShop 1.4, havia um formulário "Pegador de cor" no rodapé da lista de combinações, na qual você poderia escolher mostrar um pegador de cor ou não na página do produto.

Desde o PrestaShop 1.5, esta opção foi movida e melhorada. Quando estiver criando um novo atributo (no menu "Catálogo", página "Atributos e Valores"), você pode usar a lista de "Tipo de atributo" para escolher entre exibir uma lista, uma lista de botões, ou um pegador de cor.

### Método Automático <a href="#gerenciamentodosprodutos-metodoautomatico" id="gerenciamentodosprodutos-metodoautomatico"></a>

Se você tiver muitas versões ou variedades diferentes do produto, você pode usar o "Gerador de Combinações de Produto". Esta ferramenta permite a você gerar automaticamente todas as combinações e possibilidades.

Clicar no "Gerador de combinações do produto" leva você ao formulário de conclusão.

\- Imagem -

\- I -

Uma janela de aviso pode aparecer, dizendo "Você perderá todas as suas modificações não salvas. Você tem certeza de que gostaria de prosseguir?" isto significa que algumas combinações de seu produto foram criadas. Se você confirmar, suas combinações não salvas serão deletadas. Seja cuidadoso, e sempre salve suas alterações antes de usar o gerador!

No lado esquerdo desta página estão seus atributos e seus valores. Selecione as combinações clicando no nome dos valores (se quiser selecionar mais de um valor, pressione a tecla Ctrl enquanto clica), então clique em "Adicionar".\
Por exemplo, você pode selecionar os valores, "Azul", "P, M, G".\
Para desfazer a seleção de um atributo, simplesmente selecione seus valores e clique en "Deletar".

Assim que as variedades tiverem sido selecionadas, você pode editar o impacto éo preço e do peso do produto em cada seleção. Você não precisa: eles pode simplesmente ter o mesmo preço e peso.\
Insira a quantia de cada produto no campo "Quantidade padrão" no rodapé. Tenha cuidado, é necessário ter o mesmo para todas as combinações. Por exemplo, 200 produtos em cada combinação = 2 cores \* 1 tamanho \* 200 = 400 itens ao todo.\
Você pode adicionar uma referência padrão para esta combinação se isso facilitar suas necessidades administrativas.\
Clique no botão "Gerar estas Combinações", e o PrestaShop envia você de volta na aba "Combinações", com todas as combinações geradas. Se você precisar, você pode editar agora um por um.

Como você pode ver,  o gerador de combinação ajuda você a salvar muito tempo quando você tiver muitos atributos para montar, como tamanhos e materiais. Isso cria automaticamente todas as combinações possíveis, que então aparecerá na página pública do produto, na aba "Combinações" (se o tema suportar isso).\
Se você não quiser manter todas as combinações geradas ou se elas não são iguais (referências, preços, datas disponíveis diferentes...), você pode deleta-las (ícone da lixeira) or modifica-las (ícone do arquivo) da lista de combinação do produto. O ícone da estrela torna a combinação selecionada a padrão - no caso a que fica em azul.

### Gerenciamento da Quantidades dos Produtos <a href="#gerenciamentodosprodutos-gerenciamentodaquantidadesdosprodutos" id="gerenciamentodosprodutos-gerenciamentodaquantidadesdosprodutos"></a>

Quantidade de produtos são gerenciadas em uma única aba. A maneira que isso funciona é bem fácil: a página apresenta você com uma tabela de todas as combinações para o produto atual (se não houverem combinações, a tabela simplesmente tem uma linha). Cabe a você configurar o estoque inicial de todas as combinações. PrestaShop utilizará isso para determinar quando um produto estará próximo de ficar sem estoque ou não está mais disponível.

#### Opções de Gerenciamento do Estoque <a href="#gerenciamentodosprodutos-opcoesdegerenciamentodoestoque" id="gerenciamentodosprodutos-opcoesdegerenciamentodoestoque"></a>

A aba quantidades suporta este recurso de gerenciamento de estoque avançado, se ativado. Isto significa que as combinações do produto atual estão distribuídas entre diferentes armazéns, PrestaShop pode lidar com a locação de cada combinação, mesmo em um armazém específico.

\- Imagem -

Por padrão, você tem que gerenciar as quantidades do produto selecionado, a partir desta página. Com o recurso do gerenciamento avançado de estoque ativado, você pode confiar no recurso de gerenciamento de estoque da PrestaShop para cuidar disto.

Para usar o gerenciamento avançado de estoque para o produto atual, marque a opção "Eu quero usar o sistema de gerenciamento de estoque avançado para este produto". Assim que isto for feito, uma opção estará disponível: "Quantidades disponíveis para o produto atual e suas combinações são baseadas no estoque em armazém". Clique na opção, e você não poderá editar mais as quantidades do atual produto a partir da página "Quantidades": o produto agora depende do seu sistema de gerenciamento de estoque.

#### Quando fora de estoque <a href="#gerenciamentodosprodutos-quandoforadeestoque" id="gerenciamentodosprodutos-quandoforadeestoque"></a>

A opção "Quando fora de estoque" permite você a configurar o comportamento da plataforma PrestaShop quando o produto estiver sem estoque: negar ordens (o produto não está mais disponível para venda) ou permitir o pedido (na verdade, você está fazendo pré-vendas). A terceira e opção padrão usa simplesmente a configuração padrão global (menu "Configurações", página "Produtos", seção "Estoque do Produto", opção "Permitir vender produtos sem estoque").

#### &#x20;Configurações de Disponibilidade <a href="#gerenciamentodosprodutos-configuracoesdedisponibilidade" id="gerenciamentodosprodutos-configuracoesdedisponibilidade"></a>

No rodapé da página, você pode configurar o comportamento padrão da plataforma PrestaShop dependendo da disponibilidade do produto atual.

\- Imagem -

As opções são:

* &#x20;**Texto exibido quando em estoque**. Permite você a exibir uma mensagem para seu visitante quando seu produto estiver em estoque, por exemplo "Item disponível". Reassegura eles que sua loja pode enviar imediatamente o produto.
* **Texto exibido quando pode ser retornado**. Permite que você mostre uma mensagem para seus visitantes quando seu produto está fora de estoque mas eles ainda podem compra-lo (como configurado utilizando o seletor "Quando estiver sem estoque"), por exemplo "Reserve agora!". Isso reassegura eles de que sua loja enviara o produto imediatamente quando estiver em estoque.

&#x20;Você também pode modificar as configurações gerais aplicadas a todos os seus produtos: a opção padrão é a de negar os pedidos, mas isso pode ser modificado na configuração "Produtos" (opção "Permitir vender produtos sem estoque"), que pode ser completamente explicado no capítulo "Entendendo as Configurações" deste guia.

#### Configurando as Imagens do Produto <a href="#gerenciamentodosprodutos-configurandoasimagensdoproduto" id="gerenciamentodosprodutos-configurandoasimagensdoproduto"></a>

&#x20;A aba "Imagens" à esquerda é para incluir fotos na página do seu produto. Você deveria enviar todas as Imagens deste produto, incluindo todas as suas combinações (cor, tamanho, formato, etc.).

&#x20;\- Imagem -

&#x20;Para adicionar uma ou mais imagens ao seu produto:

1. &#x20;Clique no botão "Adicionar arquivos" e então selecione pelo menos um arquivo do seu computador para enviar. Você pode selecionar quantas imagens forem necessárias enquanto mantiver a tecla Ctrl pressionada enquanto estiver selecionando os arquivos, ou você pode fazer sua seleção uma por uma. A plataforma PrestaShop exibirá as imagens escolhidas em uma lista, com seus tamanhos e um botão para remover algumas.\
   O tamanho máximo padrão para uma imagem é configurado pela plataforma PrestaShop de acordo com as configurações do PHP do seu servidor. Este tamanho pode ser diminuído na pagina de configurações "Imagens", na seção "Imagens do produto".
2. Dê um título à imagem. Será exibido se a imagem não puder ser exibida - o que pode ser muito bom para sua otimização do motor de busca.
3. Clique no botão de enviar para disponibilizar seu arquivo online.
4. As imagens enviadas aparecerão em uma tabela abaixo do botão. Se você tiver mais de uma imagem, você pode escolher qual imagem deve ser utilizada como a padrão/ de capa clicando no botão vermelho "sem registro" e tornando-o em uma marcação. Essa imagem de capa também aparecerá automaticamente na página do produto da sua loja.\
   Você pode clicar numa miniatura para exibir a imagem em tamanho completo.

&#x20;Assim que você tiver enviado todas as suas imagens do produto, você pode modificar a ordem das imagens clicando, arrastando e soltando a linha da tabela quando o cursor do mouse virar un cursor "móvel".

#### &#x20;Configurando os Recursos do Produto <a href="#gerenciamentodosprodutos-configurandoosrecursosdoproduto" id="gerenciamentodosprodutos-configurandoosrecursosdoproduto"></a>

&#x20;A aba "Recursos" é onde você especifica os recursos do seu produto (p. ex. peso, material, país de origem, etc.).

&#x20;\- Imagem -

&#x20;Quando você cria recursos e valores (p. ex. lã e materiais de micro-fibras), você os colocara nos produtos quando for apropriado. Isto significa que você não tem que preencher os recursos para cada um de seus produtos mas ao invés disso simplesmente preencha o valores necessários e altere o produto mais tarde.

O mecanismo da PrestaShop se baseia inteiramente nos recursos do produto: é isso que é comparado.

Também, já que a comparação funciona de acordo com a categoria, você deveria ter certeza de que todos os produtos em uma categoria compartilham os mesmos recursos, com vários valores para serem comparados entre si.

Tenha ciência de que **ao contrário das combinações, estes valores não mudam, e são válidos para o produto em geral** (ou seja: todas as suas combinações compartilharão os mesmos recursos).

#### &#x20;Criando um recurso <a href="#gerenciamentodosprodutos-criandoumrecurso" id="gerenciamentodosprodutos-criandoumrecurso"></a>

&#x20;Antes de adicionar um recurso a um produto, você deve cria-lo para o uso geral em sua loja. Ou você vai para a página "Recursos" do menu "Catálogo", ou diretamente clicando no botão "Criar um novo recurso". Um aviso aparecerá, "Você perderá todas as modificações não salvas. Você tem certeza de que deseja continuar?" - tenha certeza que todas as suas modificações estão salvas antes de validar.

&#x20;Recurso e criação de recurso são explicados em detalhe na seção dedicada do guia.

#### &#x20;Atribuindo um valor e recurso para um produto <a href="#gerenciamentodosprodutos-atribuindoumvalorerecursoparaumproduto" id="gerenciamentodosprodutos-atribuindoumvalorerecursoparaumproduto"></a>

&#x20;Nós assumiremos aqui que você já configurou todos os seus recursos e valores de recurso.

&#x20;Na aba à esquerda do produto atual "Recursos", uma tabela é exibida, listando todos os recursos da sua loja. Nem todos pertencem a este produto: PrestaShop considerará relevante apenas os recursos nos quais você configurou um valor.

&#x20;Você pode configurar manualmente, no campo à direita da linha do recurso, ou você pode usar um valor pré-definido (como configurado na criação do recurso) se houver qualquer disponível. Se nenhum valor estiver disponível para um recurso, o texto "N/A" aparece (abreviação para "não aplicável"), seguido de um botão "Adicionar valores pré-definidos primeiramente".

&#x20;Se você escolheu utilizar um valor customizável, não esqueça de configura-lo para todos os idiomas que sua loja suporta. Use o seletor de código de idioma para alterar o idioma.

&#x20;Se houverem valores predefinidos disponíveis, eles aparecerão numa lista. Simplesmente clique nela e escolha o valor correto.

&#x20;Assim que você tiver configurado todos os recursos relevantes, salve suas alterações para vê-las imediatamente aplicadas na primeira página.

&#x20;Lembre-se: se um recurso não tem nenhum valor atribuído, ele não será considerado para este produto, e não estará visível na sua loja.

#### &#x20;Gerenciamento de Customização <a href="#gerenciamentodosprodutos-gerenciamentodecustomizacao" id="gerenciamentodosprodutos-gerenciamentodecustomizacao"></a>

&#x20;PrestaShop faz com que seja possível para seus clientes customizarem o produto que eles comprarão.

&#x20;Exemplo: Você é um vendedor de jóias e seus clientes podem escrever as jóias com um texto ou uma imagem. Seus clientes podem enviar o texto e/ ou a imagem quando eles fizerem a compra.

&#x20;A vantagem desta função é que ela oferece aos seus clientes um serviço pessoal, que eles sem dúvida gostarão!

&#x20;Vamos olhar como configurar esta fincão. Na aba "Customização" à esquerda, você pode indicar que tipo de contexto (arquivo e/ ou texto) pode ser personalizado.

&#x20;\- Imagem -

* &#x20;**Campos de arquivo**. Coloca a quantidade de botões de enviar arquivo na página do pedido. Cada botão aceita apenas um arquivo, então coloque quantos botões você permite seu cliente a enviar os arquivos.
* **Campos de texto**. Coloca a quantidade indicada de campos de texto na página do pedido. Você pode adicionar quantos campos forem necessários. Exemplo: se você permitir seu cliente usar um texto se 5 linhas com cada linha limitada por 14 caracteres, você pode adicionar 5 campos e indicar a quantidade de caracteres permitidos no texto do campo. Você não pode limitar a quantidade de caracteres no texto.

&#x20;Quando você tiver adicionado o número necessário para cada campo, clique em "Salvar e continuar". A página recarregará e mostrará quantos campos de texto forem necessários. Preencha cada um deles com o texto apropriado: isto será um indicador para o cliente, então seja bem específico sobre o que você espera.

&#x20;Por exemplo, se você permitir imagens para a capa de um livro, você poderia utilizar o seguinte:

* &#x20;"Capa da frente (20.95 x 27.31 cm, colorido)".
* "Capa de trás (20.95 x 27.31 cm, preto e branco)".
* "Espinha (20.95 x 1.716 cm, colorido)".

&#x20;O mesmo para o texto: se os clientes podem escrever palavras a um produto, você poderia usar o seguinte:

* &#x20;"Primeira linha (24 caracteres)".
* "Segunda linha (24 caracteres)".
* "Última linha, assinatura (16 caracteres)".

&#x20;**Removendo campos**. Se no fim você adicionou muitos campos, simplesmente altere o número de campos necessários para cada um dos dois tipos e clicar em "Salvar e continuar". A página recarregará com a quantidade correta de campos, com os primeiros preservados.

&#x20;Assim que todos os campos de texto tiverem sido preenchidos, não esqueça de salvar suas alterações.

#### &#x20;Do lado do cliente <a href="#gerenciamentodosprodutos-doladodocliente" id="gerenciamentodosprodutos-doladodocliente"></a>

&#x20;Assim que um produto tiver suas propriedades customizadas configuradas, a página do produto terá uma nova aba, próxima da aba "Mais informações": "Customização do produto".

&#x20;O cliente deve escolher o(s) arquivo(s) e/ ou adicionar algum texto e salva-los antes de adicionar o produto no carrinho.

&#x20;A(s) imagem(ns) e texto(s) customizado(s) aparecerão no carrinho final.

&#x20;O resto do processo de compra é o mesmo que o habitual.

#### &#x20;Do lado do vendedor <a href="#gerenciamentodosprodutos-doladodovendedor" id="gerenciamentodosprodutos-doladodovendedor"></a>

&#x20;Assim que o pedido tiver sido validado pelo cliente, o vendedor recebe uma notificação do pedido na plataforma.

&#x20;Ele pode verificar no pedido, o que indicara a(s) imagem(ns) e o(s) texto(s) na lista de produtos, para cada produto. O vendedor então simplesmente tem que baixar a(s) imagem(ns) (simplesmente clicando na imagem na ordem) ou copiar/ colar o texto e usar aquilo que está na ferramenta de customização.

&#x20;O resto do processo de compra e entrega é o mesmo que o habitual.

### &#x20;Gerenciamento dos anexos <a href="#gerenciamentodosprodutos-gerenciamentodosanexos" id="gerenciamentodosprodutos-gerenciamentodosanexos"></a>

&#x20;A plataforma PrestaShop habilita você a fazer alguns arquivos para seus clientes antes de fazerem o pedido. Isto é feito na aba "Anexos" à esquerda.

&#x20;\- Imagem -

&#x20;Por exemplo, digamos que você venderá eletrônicos, e você gostaria de convencer seus clientes a lerem um documento em como um produto funciona. Você pose enviar um documento para isso.

&#x20;Você poderia também simplesmente ter o manual do produto em PDF diretamente disponível para baixar na página do produto.

&#x20;Adicionar um anexo é muito rápido:

1. &#x20;Preencha o nome do arquivo do seu anexo (não precisa ser o mesmo que p nome original do arquivo).
2. Dê a ele uma descrição. Isto ajudará você a destinguir entre os arquivos que você enviou com certeza.
3. Clique em "Adicionar arquivo" para selecionar um arquivo no seu computador para enviar.
4. O mais cedo que você escolher o arquivo, PrestaShop o enviará, então mostrará a lista. O anexo aparecerá na lista "Anexos disponíveis": você tem que seleciona-lo e clicar em "Adicionar" para movê-lo para a lista "Anexos para este produto".
5. Salve o seu produto com o botão "Salvar" ou o "Salvar e continuar".

&#x20;Agora a aba "Baixar" aparecerá na página do produto (se o tema suportar isso), e seus clientes poderão baixar o(s) arquivos(s) que você enviou.

&#x20;Se você precisa remover um anexo, selecione-o no seletor "Anexos para este produto" e clique no botão "<-Remover". O arquivo será movido para ser configurado para o seletor "Anexos disponíveis" se você precisar coloca-lo novamente mais tarde.

&#x20;Você pode ver todos os seus arquivos anexados, adicionar mais alguns e remover alguns, através da página "Anexos" no menu "Catálogo". Isto também fará possível usar os anexos que você já enviou outros arquivos: se você precisa aplicar o arquivo associados com vários produtos, você precisará enviar apenas uma vez.

### &#x20;Configuração do Fornecedor do Produto <a href="#gerenciamentodosprodutos-configuracaodofornecedordoproduto" id="gerenciamentodosprodutos-configuracaodofornecedordoproduto"></a>

&#x20;Indicar o fornecedor do produto não é realmente importante para seus clientes (muito menos do que o fabricante em qualquer caso), mas pode se tornar parte essencial do seu gerenciamento interno, gerenciando seu estoque: você simplesmente tem que saber de quem você está comprado o produto. O fornecedor do produto atual é para ser escolhido da aba "Fornecedores" à esquerda.

&#x20;\- Imagem -

Você não pode usar este recurso se você não tiver pelo menos um fornecedor registrado na sua loja. Fornecedores são criados na página "Fornecedores", no menu "Catálogo".

&#x20;O processo completo de criação de fornecedor é explicado em detalhes no capítulo atual deste guia. Você pode acessar a pagina de criação diretamente clicando no botão "Criar um fornecedor".

Associando o produto atual com um ou mais fornecedores é muito fácil: simplesmente clique na caixa correspondente ao fornecedor, e salve suas alterações.

&#x20;Se o produto é associado com mais de um fornecedor, você pode escolher qual deveria seria o padrão marcando a bolinha à direita. Observação: os botões"Padrão" estão indisponíveis por padrão. Para seleciona-los, você deve primeiro clicar no botão "Salvar e continuar" para poder selecionar outro fornecedor como padrão.

#### &#x20;Referência (s) do produto <a href="#gerenciamentodosprodutos-referencia-s-doproduto" id="gerenciamentodosprodutos-referencia-s-doproduto"></a>

&#x20;A página do fornecedor do produto também tem uma tabela que permite você a configurar a referência e o preço unitário/ moeda exata para cada combinação do produto. Se o produto tem mais do que um fornecedor, a tabela abre apenas a combinação atrelada ao primeiro fornecedor, os outros fechados por padrão. Clique no nome do fornecedor para abrir sua tabela de referências, e fechar as outras.

&#x20;\- Imagem -

### &#x20;Gerenciamento de Estoques (avançado) <a href="#gerenciamentodosprodutos-gerenciamentodeestoques-avancado" id="gerenciamentodosprodutos-gerenciamentodeestoques-avancado"></a>

&#x20;Assim que você habilitar a opção de gerenciamento avançado de estoque (na página fe configuração "Produtos"), esta nova aba fica disponível para todos os produtos, e permite a você indicar em qual armazém o produto atual está armazenado.

&#x20;\- Imagem -

Você não pode usar este recurso se você não tiver pelo menos um armazém registrado na sua loja. Armazéns são criados na página "Armazéns", no menu "Estoque".

O processo de criação completa do armazém é explicado em detalhes em outro capítulo deste guia.\
Você pode acessar o formulário de criação clicando no botão "Criar novo armazém".

A aba "armazém" apresenta para você uma tabela que permite você a configurar o local preciso para cada combinação do produto (se qualquer) em cada armazém. Se você tiver registrado mais de um armazém, a tabela apenas mostrará o primeiro por padrão, os outros fechados por padrão. Clique no nome de um armazém para abri-lo em uma sub tabela, e fechar as outras.

&#x20;Para cada armazém, você pode configurar qual variação do produto atual é armazenada, e um campo de texto permite a você indicar precisamente onde é armazenado no armazém. Você pode escrever qualquer coisa no campo: "5° corredor", "Próximo do álbum Radiohead", "A07 E08 H14", ou qualquer coisa que ajude você ou sua equipe de empacotamento a encontrar o produto rapidamente.

## &#x20;Criando um Pacote de Produtos <a href="#gerenciamentodosprodutos-criandoumpacotedeprodutos" id="gerenciamentodosprodutos-criandoumpacotedeprodutos"></a>

&#x20;Você pode querer vender um kit de produtos feito de vários itens. P. ex.: um kit inicial de computador composto pelo computador, um monitor, e uma impressora. PrestaShop facilita para você criar um produto "kit" e adicionar outros produto do seu catálogo para este kit.

&#x20;Kits permitem que você simplifique a preparação dis pedidos. Eles também permitem que os clientes tenham vantagem como preços especiais e ofertas.

Você não pode adicionar combinações ou produtos virtuais ao kit.

Se você precisar ter kits com combinações, você terá que criar produtos únicos para cada combinação. Isto é uma limitação conhecida que será corrigida na próxima versão do PrestaShop.

Você não pode adicionar um kit existente em um novo kit, ou importe o conteúdo de um kit existente em um novo kit.

&#x20;O processo para criar um kit é similar ao de criar um produto regular:

1. &#x20;Vá a página "Produtos", no menu "Catálogo".
2. Clique no botão "Criar novo".
3. A partir da aba "Informação" à esquerda, mude o tipo do produto para "Kit de produtos existentes".

Abaixo da opção "Tipo", uma nova seção aparecerá. Tem apenas dois campos de texto e um botão:

* O primeiro campo é usado para procurar por produtos que já estão registrados na sua loja.
* O segundo campo é usado para indicar a quantidade do produto escolhido a ser adicionada ao kit.
* O botão adiciona o produto ao pacote.

&#x20;\- Imagem -

&#x20;Você pode adicionar quantos produtos você quiser no kit.

&#x20;Você pode remover um produto do kit simplesmente clicando no ícone da lixeira próximo do produto.

&#x20;Uma nova opção também aparecerá na "Aba quantidades": é para ajudar você a gerenciar ad quantidades do seu kit.

### &#x20;Quantidades do kit <a href="#gerenciamentodosprodutos-quantidadesdokit" id="gerenciamentodosprodutos-quantidadesdokit"></a>

&#x20;Quando você está criando um kit de produtos, PrestaShop precisará saber como lidar com o estoque. Na aba "Quantidades", sob "Quantidade de kits", você deve escolher uma das seguintes opções:

* &#x20;**Diminuir apenas o estoque do kit (comportamento padrão)**. Quando um kit é vendido, apenas o estoque do kit será impactado.
* **Diminuir apenas o estoque fos produtos no kit**. Quando o kit é vendido apenas o estoque dos produtos que o compõe será impactado.
* **Diminuir ambos**. Quando um kit é vendido, ambos os estoques do kit e de cada produto que o compõe será impactado.
* **Comportamento padrão**. Este é o comportamento padrão conforme configurado no nível loja na sua configuração de produtos. Por padrão você terá a opção "Diminuir apenas o estoque do kit" mas ele mudará de acordo com sua escolha.

&#x20;Assim que você tiver terminado com o "Kit", você pode alterar o conteúdo de todas as outras abas disponíveis como você faria com um produto comum.

## &#x20;Criando um Produto Virtual <a href="#gerenciamentodosprodutos-criandoumprodutovirtual" id="gerenciamentodosprodutos-criandoumprodutovirtual"></a>

&#x20;Sua loja pode ter (parcialmente ou exclusivamente) produtos virtuais - isso é, produtos que não são enviados, mas ao invés baixados: tickets para show, livros digitais/ arquivos PDF, serviços na vida real...

&#x20;A plataforma PrestaShop torna fácil para você criar um produto virtual.

&#x20;O processo para fazer isso é similar ao de criar um produto simples:

* &#x20;Vá à página "Produtos", sob o menu "Catálogo".
* Cliques no botão "Criar novo".
* A partir da aba "Informação" à esquerda, altere o tipo do produto para "Produto Virtual".

&#x20;As abas à esquerda mudam:

* &#x20;A aba "Produto Virtual" aparece, a qual você será redirecionado assim que você mudar o tipo do produto.
* A aba "Enviando o produto" desaparece.

&#x20;A nova aba contém apenas uma opção primeiramente: uma opção para você indicar se o produto virtual que você está criando tem um arquivo anexado (p. ex., se seu cliente pagará para baixar algo).

* &#x20;Se não, deixe a opção como está: você está vendendo um serviço e nada precisa ser baixado.
* Se sim, clique na opção "Sim".

&#x20;\- Imagem -

&#x20;Quando você clica em "Sim", a plataforma PrestaShop abre um novo formulário dentro da aba, a partir do qual você pode enviar o arquivo que você pretende vender:

* &#x20;**Nome do arquivo**. O nome do arquivo. Este campo é automaticamente preenchido depois do arquivo ter sido enviado. Não é recomendado altera-lo para outro valor.
* **Arquivo**. Clique no botão "Escolher arquivo" para encontrar o arquivo no seu disco rígido. Tão cedo quanto você tiver selecionado, o envio começa.

A configuração do tamanho máximo do arquivo a ser enviado depende da configuração do seu servidor, e não pode ser aumentado a partir do PrestaShop.

&#x20;Se você tem acesso ao arquivo php.ini do seu servidor, estes são os valores que você deveria mudar:

&#x20;\- upload\_max\_filesize = 20M

&#x20;\- post\_max\_size = 20M

Se você não tiver acesso ao arquivo php.ini, entre em contato com o host da sua loja.

Você deveria comprimir seu arquivo no formato zip, para evitar que o navegador confunda-o com formatos de arquivos .exe ou .jpg. Navegadores baixam automaticamente arquivos zip para o cliente, sem perguntar nada.

Se você está vendendo uma imagem em alta resolução, envia-la dessa maneira não previne você de enviar a miniatura da imagem na aba "Imagens" à esquerda.

1. **Número de downloads permitidos**. Você pode definir o número de vezes que o arquivo pode ser baixado após o cliente compra-la. Você pode preferir limitar para 1, ou 5 vezes. Se você quiser manter ilimitada, configure para 0.
2. **Data de Expiração**. Arquivos virtuais podem ser de natureza promocional, ou perderem seu valor de venda após certa data. Se for assim, você pode configurar a data de expiração após a qual o produto não estará mais disponível na sua loja. Deixe-o em branco se não houver data de expiração.
3. **Número de dias**. Você pode configurar o número de dias após o qual o link de download parará de funcionar. Se não houver limite, configure-o com 0.

&#x20;Assim que você tiver finalizado com a aba "Produto Virtual", você pode editar todas as outras abas disponíveis como você faria com um produto comum.
