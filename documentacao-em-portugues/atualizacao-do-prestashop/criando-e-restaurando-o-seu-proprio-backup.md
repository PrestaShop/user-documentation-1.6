# Criando e restaurando o seu próprio backup

**Sumário**

/\*\<!\[CDATA\[\*/\
div.rbtoc1597243848511 {padding: 0px;}\
div.rbtoc1597243848511 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597243848511 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Criando e restaurando seu próprio backup](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-Criandoerestaurandoseuprópriobackup)
  * [Criando seu backup](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-Criandoseubackup)
    * [Copiando seus arquivos](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-Copiandoseusarquivos)
    * [Copiando seu banco de dados](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-Copiandoseubancodedados)
      * [Usando a ferramenta de backup de banco PrestaShop](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-UsandoaferramentadebackupdebancoPrestaShop)
      * [Usando o phpMyAdmin](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-UsandoophpMyAdmin)
      * [Usando a ferramenta de backup da sua hospedagem](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-Usandoaferramentadebackupdasuahospedagem)
  * [Restaurando o backup](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-Restaurandoobackup)
    * [Limpando seu servidor](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-Limpandoseuservidor)
      * [Criando a página de manutenção](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-Criandoapáginademanutenção)
      * [Apagando arquivos](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-Apagandoarquivos)
      * [Apagando dados](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-Apagandodados)
    * [Restaurando dados e arquivos](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-Restaurandodadosearquivos)
      * [Restaurado arquivos](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-Restauradoarquivos)
      * [Restaurando dados](criando-e-restaurando-o-seu-proprio-backup.md#Criandoerestaurandooseuprópriobackup-Restaurandodados)

## Criando e restaurando seu próprio backup <a href="#criandoerestaurandooseupropriobackup-criandoerestaurandoseupropriobackup" id="criandoerestaurandooseupropriobackup-criandoerestaurandoseupropriobackup"></a>

Se você está atualizando sua instalação do PrestaShop usando o método automático ou manual, você deve certificar-se de que você tem seu próprio conjunto de dados de backup, um que você pode confiar e que você pode obter de volta em seus próprios termos.

Ao realizar um upgrade da loja, é altamente aconselhável fazer o backup somente depois que a loja foi colocado em modo de manutenção. Dessa forma, você tem certeza de que nenhum dado do cliente for perdido, se você tiver que reverter o upgrade para o backup. Não realize a atualização antes de ambos os arquivos e dados tenham sido devidamente copiados para seu computador.

Nos processos descritos neste capítulo você terá que transferir arquivos usando um cliente FTP, fazer download de dados SQL de um servidor web usando ferramentas on-line e até mesmo apagar todos os seus arquivos on-line e de dados. Não tente fazer isso se você não tem uma boa compreensão destas ferramentas e tecnologias. Se você tem (uma loja exemplo, ou se sua loja está desconfigurada após uma falha na atualização), peça ajuda de um técnico, e separe um tempo para realizar cada etapa completamente. Se não, você pode perder sua loja para sempre.

### Criando seu backup <a href="#criandoerestaurandooseupropriobackup-criandoseubackup" id="criandoerestaurandooseupropriobackup-criandoseubackup"></a>

Primeiro, crie uma pasta em seu computador, onde você irá armazenar ambos os seus arquivos do PrestaShop e dados. Coloque a data atual no nome da pasta, a fim de saber exatamente de quando o backup é.

#### Copiando seus arquivos <a href="#criandoerestaurandooseupropriobackup-copiandoseusarquivos" id="criandoerestaurandooseupropriobackup-copiandoseusarquivos"></a>

Isto é realmente fácil:

1. Conecte em seu servidor web usando qualquer cliente de FTP, como o FileZilla.
2. Baixar todos os arquivos da pasta online do PrestaShop na sua pasta de backup local.

Este processo pode demorar algum tempo, dependendo da velocidade do seu servidor. PrestaShop 1.6 tem cerca de 10.000 arquivos em 2.500 pastas, e isso sem contar seus próprios arquivos (imagens de produtos, temas, módulos, etc.), ou imagens de seus visitantes. Deixe o processo chegar até a conclusão; não toque no seu cliente FTP até que seja concluído.

#### Copiando seu banco de dados <a href="#criandoerestaurandooseupropriobackup-copiandoseubancodedados" id="criandoerestaurandooseupropriobackup-copiandoseubancodedados"></a>

Enquanto os arquivos estão sendo baixados, você pode usar o tempo para fazer backup de seus dados. Você tem um duas maneiras de fazer isso ...

**Usando a ferramenta de backup de banco PrestaShop**

O PrestaShop 1.6 tem a sua própria ferramenta de backup, chamado "DB Backup" é localizado no menu "Parâmetros avançados". Essa ferramenta é explicada em detalhes no capítulo "Entendendo Os parâmetros avançados" do Guia do Usuário do PrestaShop 1.6, mas aqui está a essência do mesmo:

1. Leia o aviso legal, e clique no botão "Eu li o aviso legal - Criar um novo backup". O PrestaShop cria um arquivo zip de todas as suas tabelas de banco de dados.
2. Clique no último arquivo de backup na tabela abaixo do aviso legal. Isso deve fazer o seu navegador baixar o arquivo de backup, normalmente denominado como "1349964600-71d48cfe.sql.bz2". Salve o arquivo na pasta de backup.

**Usando o phpMyAdmin**

Se você prefere confiar no recurso de backup do phpMyAdmin em vez da ferramenta do PrestaShop, você pode! Aqui está o processo a seguir:

1. Faça o login no phpMyAdmin no seu servidor de hospedagem.
2. A partir da tela de login principal, selecione "Bases de dados".
3. Clique no nome do banco de dados do PrestaShop para abri-lo.
4. Na tela de banco de dados, clique na guia "Exportar" no conjunto superior de guias.
5. Na tela de exportação:
   1. Certifique-se de todas as tabelas do PrestaShop estão selecionados, e apenas elas. Elas devem começar com o prefixo ps\_ (ou qualquer prefixo que você escolheu para usar durante a instalação PrestaShop).
   2. Verifique se o botão de opção "SQL" é selecionado.
   3. Na seção "Estrutura", marque as seguintes caixas:\
      &#x20;\- "Estrutura".\
      &#x20;\- "Adicionar DROP TABLE / VIEW / procedure / function".\
      &#x20;\- "Adicionar IF NOT EXISTS".\
      &#x20;\- "Adicionar AUTO\_INCREMENT".\
      &#x20;\- "Incluir nomes de campo e tabela com aspas".
   4. Na seção "Dados", marque, pelo menos, a seguinte caixa:\
      &#x20;\- "Dados".
   5. Na seção "Salvar como arquivo" :\
      &#x20;\- Maque "Salvar como arquivo".\
      &#x20;\- Deixar o modelo sozinho (geralmente, "\_\_\_\_").\
      &#x20;\- Marque a caixa de "zipado" "compactado", a fim de comprimir o arquivo antes de baixá-lo.
   6. Clique no botão "Executar".
6. O navegador deve iniciar o download do arquivo de dados. Salve o arquivo na pasta de cópia de segurança do seu computador.

Se o servidor é demasiado fraco para permitir que você exportar todas as suas tabelas de uma vez, quebre o seu backup em vários arquivos. Por exemplo, escolher os primeiros 20 tabelas de dados ps\_ e exporte, indicando claramente no nome do arquivo que é o primeiro de vários. Uma vez que esses arquivos estão seguros no seu computador, faça o mesmo para os próximos 20 tabelas, e assim por diante, sem esquecer de indicar a sua posição no nome do arquivo.

**Usando a ferramenta de backup da sua hospedagem**

Sua hospedagem pode não deixar o phpMyAdmin disponível para você, e em vez disso você pode ter que usar uma ferramenta personalizada, ou qualquer outra ferramenta menos conhecida, como a integrada no cPanel. Leia a documentação do seu servidor de hospedagem. O objetivo é conseguir uma exportação seja dos seus dados em formato SQL, comprimido ou não.

### Restaurando o backup <a href="#criandoerestaurandooseupropriobackup-restaurandoobackup" id="criandoerestaurandooseupropriobackup-restaurandoobackup"></a>

Após uma atualização automática que falhou (que é a única razão pela qual você deve reverter a atualização), se você ainda puder acessar a página de administração do PrestaShop e usar o módulo 1-Click upgrade, use a ferramenta "Revert" desse módulo, a fim de iniciar o processo que restaura ambos os arquivos e dados que ele fez backup quando você começou a atualização automática. Leia o "Atualização automática" deste guia para obter mais informações sobre esse processo.\
Se você não puder acessar a administração ou o módulo, ou se você simplesmente não usar o módulo 1-Click upgrade para atualizar para a versão mais recente do PrestaShop, em seguida, siga as instruções nesta seção.

Um problema com o módulo 1-Click upgrade é que você tem que estar logado à administração do PrestaShop se você quiser começar a reverter para a versão anterior - e em algumas configurações imprevisíveis, a atualização pode impedi-lo de voltar a entrar de novo, ou mesmo tornar a administração inutilizável (nota: esvaziar o cache do navegador e recarregue a administração várias vezes antes que você considera-o inutilizável ... pode ser simplesmente uma questão de CSS temporário).

É por isso que o módulo 1-Click upgrade insiste que você execute seus próprios backups: antes de tentar qualquer upgrade, você deve ter em seu disco rígido uma cópia exata de sua loja. Em resumo:

* Uma pasta (ou um arquivo zip), que contém todos os arquivos do PrestaShop, especialmente aqueles específicos para a sua instalação: arquivos de configuração, temas, módulos, imagens, uploads de usuários, modelos PDF e e-mail, classes personalizadas, etc.
* Uma cópia completa do seu banco de dados, em um arquivo SQL ou em um arquivo zip.

Esta cópia local do seu site deve ser extremamente recente: na melhor das hipóteses, ele deve ter sido feita logo depois de colocar PrestaShop na manutenção, e antes de começar qualquer script de atualização (automática ou manualmente). Dessa forma, você vai garantir que você pode voltar para a versão mais recente da sua loja, e não perder quaisquer dados (usuários, vendas, estatísticas, etc.).

#### Limpando seu servidor <a href="#criandoerestaurandooseupropriobackup-limpandoseuservidor" id="criandoerestaurandooseupropriobackup-limpandoseuservidor"></a>

Agora, você tem uma cópia local completa e recente da sua loja, na sua versão anterior, e sua tentativa de trazer o seu site on-line para última versão do PrestaShop falhou, resultando em uma administração inútil (o front-end deve estar inacessível, uma vez que sua loja deve estar no modo de manutenção). Voltar para a versão anterior significa restaurar sua cópia local em seu servidor on-line, e que implica fazer isto a partir de uma pasta limpa, a fim impedir que os dados antigos e novos misturarem e ainda desconfigure seu site.

Isto significa apagar todos os arquivos em seu servidor, e excluir todas as tabelas de dados no banco de dados.

Não se preocupe: uma vez que todos esses arquivos e dados já estão sãos e salvos no seu computador, você será capaz de restaurá-los rapidamente. Mas os visitantes vão continuar a entrar na sua loja, você tem que exibir uma página de manutenção personalizada enquanto você está trabalhando para restaurar a sua loja.

**Criando a página de manutenção**

Revertendo sua loja para sua versão anterior pode levar algum tempo, dependendo de quão grande é a sua loja é, e, portanto, sobre o número de arquivos e a quantidade de dados que você tem que transferir. Por isso, é importante ter uma página de manutenção que não depende do PrestaShop.

Na verdade, a página de manutenção existente depende fortemente do PrestaShop para exibir algumas informações: nome da loja, logotipo da loja, tradução, arquivo CSS, meta dados, etc. Mesmo que sua loja está em modo de manutenção e, portanto, está exibindo a página de manutenção para os visitantes , essa página não funciona mais assim que eliminar os seus dados ... e não vai estar aqui logo que você apagar seus arquivos, como essa página é a partir do tema atual, sob o nome maintenance.tpl.

Por isso, a necessidade de uma página personalizada manutenção. Ele não tem que ser extravagante ou qualquer coisa, como o seu papel é simplesmente para ter uma mensagem rápida pedindo aos visitantes para voltarem mais tarde.

Aqui está um exemplo básico:**Sample maintenance page**

```
<!DOCTYPE html>
<html>
   <head>
     <title> Nossa loja está em manutenção </title>
   </head>
   <body>
     <P> A fim de executar a manutenção do site, a nossa loja on-line foi desligado temporariamente. </P>
     <P> Pedimos desculpas pelo inconveniente e peço que você tente novamente mais tarde. </P>
   </body>
</html>
```

Copie este código em um arquivo de texto index.html, e coloque na pasta do PrestaShop usando o cliente FTP. Na maioria dos servidores, o arquivo index.html tem precedência sobre o arquivo index.php, assim logo que você fazer upload de index.html à pasta raiz PrestaShop, sua loja deve exibir esta página de manutenção em vez de um de PrestaShop. Verifique as configurações do seu servidor para se certificar de que é assim.

**Apagando arquivos**

Conecte em seu espaço de hospedagem usando seu cliente FTP. vá para a pasta PrestaShop (se ele não está localizado na raiz), selecione todos os arquivos e pastas na pasta PrestaShop (exceto index.html, a sua página de manutenção de costume), e exclua todos. Obviamente, você só deve fazer isso se tiver certeza de que você tem uma cópia exata de seus arquivos de backup em seu computador.

Isso pode demorar alguns minutos, O PrestaShop tem mais de 7000 arquivos. Enquanto eles estão sendo excluídos, vamos eliminar as tabelas de dados (próxima seção).

**Apagando dados**

Abra o administrador do seu banco de dados - normalmente, o seu servidor de hospedagem irá fornecer-lhe com o phpMyAdmin ou qualquer outra ferramenta personalizada. Encontre o banco de dados para a instalação do PrestaShop. Selecione todas as tabelas que começam com ps\_ (ou o prefixo da tabela que você escolheu ao instalar PrestaShop); se o PrestaShop é a única ferramenta usando esse banco de dados, você pode simplesmente clicar no link "Selecionar tudo" na parte inferior das tabelas a fim de selecionar todas as tabelas rapidamente.

Em seguida, abra o "Com selecionados:" no menu suspenso na parte inferior das tabelas e selecione "Apagar". Na próxima tela, o phpMyAdmin pedirá uma confirmação: clique no botão "Sim". Mais uma vez, você só deve fazer isso se tiver certeza de que você tem uma cópia exata de suas tabelas de dados de backup em seu computador.

Permitir que o processo aconteça. Finalmente, o phpMyAdmin irá exibir o banco de dados, sem de qualquer tabela.

Seu servidor está agora vazio de qualquer arquivo do PrestaShop e os dados, exceto para o arquivo de manutenção index.html. Agora é hora de colocar a sua loja de volta novamente, desta vez com arquivo de substituição e os dados que você sabe fazer o trabalho!

#### Restaurando dados e arquivos <a href="#criandoerestaurandooseupropriobackup-restaurandodadosearquivos" id="criandoerestaurandooseupropriobackup-restaurandodadosearquivos"></a>

Assim que o seu cliente FTP fizer a exclusão dos arquivos on-line, comece a enviar os que foram armazenados em seu computador! Como este processo pode demorar algum tempo, é importante não perder alguns preciosos minutos (e, portanto, as vendas potenciais), mantendo a sua loja offline por mais tempo do que o necessário.

**Restaurado arquivos**

Este processo é tão fácil quanto o que você seguiu ao fazer backup de seus arquivos:

1. Conecte em seu servidor web usando qualquer cliente de FTP, como o FileZilla.
2. Envie todos os arquivos da pasta de backup local para a pasta online do PrestaShop.

A pasta online do PrestaShop deve estar vazia, de modo a garantir que os arquivos novos e antigos não entrem em conflito. Se você não excluir todos os arquivos on-line (depois do backup deles, é claro), você deve dizer ao seu cliente FTP para substituir qualquer arquivo existente. Você não deve manter qualquer vestígio dos arquivos da atualização que falhou.

**Restaurando dados**

O processo descrito aqui usa o phpMyAdmin, que é uma ferramenta web padrão. Se seu host faz com que você use outra ferramenta para gerenciar seus bancos de dados, você terá de adaptar este processo para essa ferramenta. Verifique a documentação do seu site de hospedagem sobre o assunto.

O processo de restauração dos dados é tão fácil quanto o que você iria seguir ao fazer backup de dados:

1. Faça o login no phpMyAdmin no seu servidor web.
2. A partir da tela de login principal, selecione "Base de Dados".
3. Clique no nome do banco de dados do PrestaShop para abrir.
4. Na tela de banco de dados, clique na guia "Importar" nas guias superiores.
5. Na tela de importação:\
   &#x20;      a) No "Arquivo para importar", clique no botão "Procurar ..." e encontre o arquivo de backup de seus dados. Ela pode ser tanto o arquivo texto (SQL), ou uma versão compactada do mesmo (.sql.zip, .sql.gzip, .sql.tar.gz, etc.).\
   &#x20;      b) Na seção "Formato", certifique-se que o formato "SQL" está selecionado.\
   &#x20;      c) Clique no botão "Executar".
6. O navegador deve começar a fazer o upload do arquivo de backup.

Se você tiver mais de um arquivo de backup de dados, importe um após o outro.

Finalmente, retire sua página de manutenção (chamada index.html). ai está: sua loja está de volta online!
