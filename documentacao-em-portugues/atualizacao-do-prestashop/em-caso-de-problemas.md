# Em caso de problemas

/\*\<!\[CDATA\[\*/\
div.rbtoc1597243848532 {padding: 0px;}\
div.rbtoc1597243848532 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597243848532 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Em caso de problemas](em-caso-de-problemas.md#Emcasodeproblemas-Emcasodeproblemas)
  * [Área administrativa instável](em-caso-de-problemas.md#Emcasodeproblemas-Áreaadministrativainstável)
  * [A página de módulos não atualizou](em-caso-de-problemas.md#Emcasodeproblemas-Apáginademódulosnãoatualizou)
  * [O tema padrão da loja não funciona mais](em-caso-de-problemas.md#Emcasodeproblemas-Otemapadrãodalojanãofuncionamais)
  * [Alguns módulos não funcionam](em-caso-de-problemas.md#Emcasodeproblemas-Algunsmódulosnãofuncionam)
  * [Módulos incompatíveis](em-caso-de-problemas.md#Emcasodeproblemas-Módulosincompatíveis)
  * [Módulo de customização com layout quebrado](em-caso-de-problemas.md#Emcasodeproblemas-Módulodecustomizaçãocomlayoutquebrado)
  * [Revertendo o banco de dados](em-caso-de-problemas.md#Emcasodeproblemas-Revertendoobancodedados)
  * [Entre em contato](em-caso-de-problemas.md#Emcasodeproblemas-Entreemcontato)

## Área administrativa instável <a href="#emcasodeproblemas-areaadministrativainstavel" id="emcasodeproblemas-areaadministrativainstavel"></a>

Ao carregar as páginas depois de fazer a atualização, algumas páginas de administração podem parecer estranhas: porque o seu navegador web armazena arquivos, ele provavelmente está usando o antigo CSS e JavaScript, em vez de carregar os novos arquivos.

Você deve recarregar a página várias vezes, ou mesmo esvaziar o cache do seu navegador, a fim de obter a interface correta. Leia como limpar o cache aqui: [http://support.google.com/accounts/bin/answer.py?hl=en\&answer=32050](http://support.google.com/accounts/bin/answer.py?hl=en\&answer=32050).

## A página de módulos não atualizou <a href="#emcasodeproblemas-apaginademodulosnaoatualizou" id="emcasodeproblemas-apaginademodulosnaoatualizou"></a>

Recarregar a página duas vezes (pressione F5) deve corrigir o problema

## O tema padrão da loja não funciona mais <a href="#emcasodeproblemas-otemapadraodalojanaofuncionamais" id="emcasodeproblemas-otemapadraodalojanaofuncionamais"></a>

O nome do tema padrão foi alterado de "prestashop" para "default". Se você estava usando o tema padrão, renomeie a pasta do tema padrão do "default" para "prestashop", e tudo deve funcionar novamente. Você pode encontrar essa pasta na sua pasta / themes.

## Alguns módulos não funcionam <a href="#emcasodeproblemas-algunsmodulosnaofuncionam" id="emcasodeproblemas-algunsmodulosnaofuncionam"></a>

Quando um módulo instalado não está dando o resultado esperado, tente desinstalá-lo, instalá-lo novamente.

## Módulos incompatíveis <a href="#emcasodeproblemas-modulosincompativeis" id="emcasodeproblemas-modulosincompativeis"></a>

Em alguns casos, os módulos podem não ser compatíveis com a versão mais recente do PrestaShop. Você deve entrar em contato com a empresa / pessoa que lhe fornece este módulo para solicitar algumas alterações no código para fazer-lo funcionar na versão atual.

## Módulo de customização com layout quebrado <a href="#emcasodeproblemas-modulodecustomizacaocomlayoutquebrado" id="emcasodeproblemas-modulodecustomizacaocomlayoutquebrado"></a>

Se a sua home page está com layout quebrado porque o bloco da característica de produtos tem seus itens empilhados em uma única coluna, então você deve reinstalar o módulo de customização do produto (A partir da aba características da loja na página de módulos).

## Revertendo o banco de dados <a href="#emcasodeproblemas-revertendoobancodedados" id="emcasodeproblemas-revertendoobancodedados"></a>

Apenas avance para este passo se você não tem outra saída.

Se a sua atualização não foi boa e você não vê qualquer outra correção do que para reverter para a versão anterior do seu banco de dados, existem duas principais formas de o fazer:

* Peça ao seu provedor de hospedagem para restaurar o backup para você.\
  Certifique-se de fornecê-lo com o último backup que você fez durante a Etapa 1 do processo de atualização!

...ou...

* Importe seus dados de backup via phpMyAdmin\
  Isso geralmente é feito pelas ferramentas de banco de dados fornecidos pelo seu provedor de hospedagem, na maioria das vezes o phpMyAdmin, com o recurso de exportação e importação.\
  Se o tamanho do seu banco de dados é muito grande, você pode encontrar uma mensagem de erro. Se assim for, você pode precisar de pedir ao seu provedor de hospedagem ajuda, alterando o tamanho máximo de upload do banco de dados.

Você vai encontrar os dados de backup na pasta / admin / backups.\
Você também pode baixar o banco de dados de dentro da sua página administrativa. Abra a página "DB Backup" no menu "Parâmetros Avançados". Escolha o seu backup mais recente do banco de dados e faça o download para o seu computador, clicando sobre ela.Normalmente levam entre 1 e 20 minutos para baixar.

## Entre em contato <a href="#emcasodeproblemas-entreemcontato" id="emcasodeproblemas-entreemcontato"></a>

Para **qualquer pedido de suporte ou de ajuda para configurar o seu site**, entre em contato conosco e descubra nossas ofertas de suporte.

Nossa equipe de suporte está à sua disposição para qualquer detalhe técnico referente à atualização da sua loja para a versão mais recente do PrestaShop.

* Por e-mail: [support@prestashop.com](mailto:support@prestashop.com)
* Por telefone: +33.1 83 64 16 54 (9 am – 6 pm Central European Time)
* [http://support.prestashop.com](http://support.prestashop.com/)
* E o sempre ajudado fórum da comunidade: [http://www.prestashop.com/forums/](http://www.prestashop.com/forums/)
