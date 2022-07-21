# Solidity Documentation

## My doc in solidity.

## Structure of a Smart Contract in Solidity.

1° Version of solidity.

2° Import of libs and codes.

3° Code of Smart Contract.

# Variables:

uint - Stores an positive Integer Value.

int - Can stores positives and negatives integer values.

string - Stores a text value.

address - Stores an wallet address value.

bool - Stores a true or false value.

bytes - Stores bytes value.




## Everything in this section can be read about in the Solidity Documentation

### <a href='https://docs.soliditylang.org/en/v0.8.15/'>Solidity Docs</a>

### Basic Solidity
- Versioning
- Compiling
- Contract Declaration
- Types & Declaring Variables
- uint256, int256, bool, string, address, bytes32
- Default Initializations
- Comments
- Functions
- Deploying a Contract
- Calling a public state-changing Function
- Visibility
- Scope
- View & Pure Functions
- Structs
- Intro to Storage
- Arrays - Dynamic & Fixed sized
- Compiler Errors and Warnings
- Memory
- Mappings
- SPDX License
- Recap
- Deploying to a "Live" network
- A testnet or mainnet
- Find a faucet here
- Connecting Metamask
- Interacting with Deployed Contracts
- The EVM






# **Variáveis built-in (msg.sender, msg.value...)**

# block.chainid

A rede principal da Ethereum mainnet possui um id 1 e uma das redes de teste chamada Rinkeby possui id 3. Enquanto outras redes EVM como a Binance possui id 56, você pode ver uma lista completa de Chain IDs em [https://chainlist.org/](https://chainlist.org/).

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FqnJ9PtHfmGZ0o4PZZ1uj%2Fimage.png?alt=media&token=da7e9cf8-6dbf-4545-9a3f-bd8579d64b1c](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FqnJ9PtHfmGZ0o4PZZ1uj%2Fimage.png?alt=media&token=da7e9cf8-6dbf-4545-9a3f-bd8579d64b1c)

# **block.coinbase**

Quando for feito o deploy do contrato que estiver sendo escrito, um minerador irá incluí-lo na blockchain e através desse parâmetro é possível interagir com esse minerador. Ou até mesmo depois quando for feita uma interação com esse contrato poderá acessar o minerador que processou essa interação.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FWx2pwgivDk6dnfoRL7oW%2Fimage.png?alt=media&token=a24e1aa7-8d76-434e-964b-f629d9703645](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FWx2pwgivDk6dnfoRL7oW%2Fimage.png?alt=media&token=a24e1aa7-8d76-434e-964b-f629d9703645)

# **block.difficulty**

O parâmetro dificuldade é o que "regula" a emissão de novas moedas dentro de uma rede baseado na quantidade de mineradores que estão trabalhando nisso e esse parâmetro está sempre sendo ajustado de acordo com a oferta e demanda de poder computacional para realizar os testes de hash. Atráves de block.difficulty é possível acessar a dificuldade de mineração no bloco atual.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2F88faZGG31Ajy4nzRNQtC%2Fimage.png?alt=media&token=d0a02b9d-a6f0-4bfb-8961-8dd451c54713](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2F88faZGG31Ajy4nzRNQtC%2Fimage.png?alt=media&token=d0a02b9d-a6f0-4bfb-8961-8dd451c54713)

# **block.gaslimit**

Quanto mais cálculos e operações um smart contract tiver, mais gas ele irá consumir. Usando esse parâmetro é possível acessar a quantidade de gas disponível no bloco atual para saber se seu contrato irá ser processado ou não.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2Fcu6xJ8dMsk7qUZrTw70u%2Fimage.png?alt=media&token=d70a209b-a12c-47b9-bdf1-22b88c425b21](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2Fcu6xJ8dMsk7qUZrTw70u%2Fimage.png?alt=media&token=d70a209b-a12c-47b9-bdf1-22b88c425b21)

# **block.number**

Retorna o numero do bloco atual, pode ser usado pra muitas coisas e uma das mais comuns é travar dinheiro até determinado bloco.

No momento em que escrevo isso o bloco atual da rede Ethereum é [13525758](https://etherscan.io/block/13525758).

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FKyFxz8usEuLtstKbq822%2Fimage.png?alt=media&token=0726ecf3-84cd-47df-8d7f-a61c613b001e](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FKyFxz8usEuLtstKbq822%2Fimage.png?alt=media&token=0726ecf3-84cd-47df-8d7f-a61c613b001e)

# **block.timestamp**

Timestamp é um formato muito conhecido para *encodar* data e hora em um formato númerico, por exemplo o timestamp de agora é: 1635696570.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FvShkXmqEtjRB8d6iIlw3%2Fimage.png?alt=media&token=943a00a3-7e11-4e1a-9bdb-4989abb23780](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FvShkXmqEtjRB8d6iIlw3%2Fimage.png?alt=media&token=943a00a3-7e11-4e1a-9bdb-4989abb23780)

# **msg.sender**

Deve-se ficar muito atento ao uso que será feito dessa instrução pois no caso de criação do contrato, msg.sender será o criador do contrato mas depois em uma interação com esse contrato msg.sender será a carteira ou outro contrato que interagiu com ele.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FzYnhnNytU3VVbaEdZqD4%2Fimage.png?alt=media&token=995b56bd-b45f-425d-a23e-6c495733923b](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FzYnhnNytU3VVbaEdZqD4%2Fimage.png?alt=media&token=995b56bd-b45f-425d-a23e-6c495733923b)

# **msg.value**

Irá acessar a quantidade de Ethers (ou outra moeda se for outra blockchain) que foi enviada em uma transação.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2Fu3bVGRiGLhjM4wisgqZb%2Fimage.png?alt=media&token=6c655189-7156-4b44-9f3a-4ebb1b0906f4](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2Fu3bVGRiGLhjM4wisgqZb%2Fimage.png?alt=media&token=6c655189-7156-4b44-9f3a-4ebb1b0906f4)

# **tx.origin**

Muito parecido com msg.sender porém refere-se somente a endereços de carteira enquanto msg.sender pode referir-se também a contratos. Para compreender o uso mais detalhado acesse **[https://github.com/w3b3d3v/gitbook-solidity/blob/main/apostila/broken-reference/README.md](https://github.com/w3b3d3v/gitbook-solidity/blob/main/apostila/broken-reference/README.md)**.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FbwIz3CwS4jxatAcRyT7s%2Fimage.png?alt=media&token=b94ba514-a862-481d-a55f-d1ff2dd24d40](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FbwIz3CwS4jxatAcRyT7s%2Fimage.png?alt=media&token=b94ba514-a862-481d-a55f-d1ff2dd24d40)

# **tx.gasprice**

Irá retornar o preço de gas da transação.

# **Arrays (Listas)**

Arrays são listas de um único tipo de dado e as utilidades e aplicações são praticamente infinitas.

# **Criando Arrays**

Usamos os sinais de colchetes como em outras linguagens porém precisamos especificar o tipo desse array primeiro, e depois o seu nome.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FCD6DCdhNIx6FJ5iXYaZs%2Fimage.png?alt=media&token=403dfcc1-fdfe-473d-95a8-8e760346b275](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FCD6DCdhNIx6FJ5iXYaZs%2Fimage.png?alt=media&token=403dfcc1-fdfe-473d-95a8-8e760346b275)

lista chamada ***saldos*** do tipo ***uint*** (números inteiros positivos).

# **Adicionando itens à lista.**

Para adicionar um registro usamos o comando *push(valor_a_ser_adicionado)* e para atualizar acessamos o indice (posição da lista) em que esse vaor está armazenado. Assim como tudo na computação, listas *começam com indice 0* então o primeiro valor estará armazenado na posição 0 e o segundo na posição 1 e assim segue.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FGMs50DRst7eq1mbCQe9Y%2Fimage.png?alt=media&token=492fb682-5016-4b9f-996a-97f6b9a5a055](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FGMs50DRst7eq1mbCQe9Y%2Fimage.png?alt=media&token=492fb682-5016-4b9f-996a-97f6b9a5a055)

# **Acessando itens.**

Para acessar os dados que estão guardados nessa lista usamos seu nome e a posição do item dentro de colchetes.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FHSVbEjVo8Jgn2gTZ9S01%2Fimage.png?alt=media&token=fedbbfc4-1432-429d-b27e-07b026e8a281](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FHSVbEjVo8Jgn2gTZ9S01%2Fimage.png?alt=media&token=fedbbfc4-1432-429d-b27e-07b026e8a281)

# **Deletando itens.**

Muito semelhante à outras linguagens para deletar um item é usado a palavra ***delete*** e a posição da lista que será apagada.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FPQt0HAyJ5mglwaNYQguA%2Fimage.png?alt=media&token=c558a206-d918-4c2f-9bd6-d754fe793911](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FPQt0HAyJ5mglwaNYQguA%2Fimage.png?alt=media&token=c558a206-d918-4c2f-9bd6-d754fe793911)

# **Arrays multidimencionais**

Parecido com tabelas ou outras estruturas multidi-mencionais como tensores, também é possível construir "listas de listas" em solidity.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2F82vMTzSEaV8JSixnNwov%2Fimage.png?alt=media&token=16b1c308-87ba-40a6-a652-ffe971c07302](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2F82vMTzSEaV8JSixnNwov%2Fimage.png?alt=media&token=16b1c308-87ba-40a6-a652-ffe971c07302)

Nesse caso temos uma lista que contém outras listas de shitcoins.

Para acessar um valor guardado em uma lista de listas precisamos encontrá-lo pelos indices da seguinte forma: ***nomedalista[primeiro_indice][segundo_indice].***

# **Controladores de Fluxo (if, for, while)**

A parte mais importante de toda programação é a lógica de como um script é programado e controladores de fluxo são os tijolos dessa construção.

# **If & else**

Usado para criar condições que devem ser atendidas para que um determinado trecho de código seja executado. Já o ***else é uma condição*** que será executado ***caso a primeira não seja***.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FAeTP2yBg62kQ2B5UKMdh%2Fimage.png?alt=media&token=cea0095a-3894-4092-b4a5-1e4d5996e406](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FAeTP2yBg62kQ2B5UKMdh%2Fimage.png?alt=media&token=cea0095a-3894-4092-b4a5-1e4d5996e406)

# **Loop for**

Quando precisamos fazer interações por vários itens dentro de um array ou mapping, ou então executar algo por um número definido de vezes podemos usar loops for.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FhKPCzAEs5xnfInKX1E8I%2Fimage.png?alt=media&token=d22e447e-aaac-4bd0-825b-715c218cc89f](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FhKPCzAEs5xnfInKX1E8I%2Fimage.png?alt=media&token=d22e447e-aaac-4bd0-825b-715c218cc89f)

*o valor de* ***i começa em zero*** e ******irá ***acrescentando 1*** até chegar no valor armazenado em ***listaDeEnderecos.length*** que é reponsável por retornar o tamanho da lista. De 1 em 1 o loop irá executar o trecho de código para cada endereço guardado na ***listaDeEnderecos.***

# **loop While**

Se precisarmos repetir um trecho de código por um número indefinido de vezes ou até que uma condição seja atingida usamos loops while.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FVWp0M6QlQQ8RzwIbbB6e%2Fimage.png?alt=media&token=e5453a24-245d-4a01-99a9-f75d9bbeff43](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FVWp0M6QlQQ8RzwIbbB6e%2Fimage.png?alt=media&token=e5453a24-245d-4a01-99a9-f75d9bbeff43)

Obs: isso pode gastar muito gás então use com muita atenção.

O loop While irá ficar rodando até que as condições pra ele parar sejam alcançadas e essa condição pode ser construída com ***if*** seguido de um ***break*** que é o código irá parar. Há outra instrução nesse código que é o ***continue***, responsável por fazer o loop "pular" para o inicio ao invés de ser executado até o final e só então recomeçar.

# **Mappings (Dicionários)**

Não é incorreto afirmar que mappings são como dicionários de outras linguagens pois também se armazena dados utilizando uma estrutura de chave-valor.

# **Criando um dicionário.**

Assim como todas as outras [variáveis em solidity](https://solidity.web3dev.com.br/apostila/tipos-de-variaveis) nós primeiros definimos o tipo do dicionário e depois seu nome. No nosso exemplo, temos um dicionário em que as ***chaves são endereços*** e os **valores são números inteiros** que representam os saldos e o mapping se chama ***balances***.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2Frd0IihTwKZszWXYWgGpP%2Fimage.png?alt=media&token=8d058cd3-5150-434f-91db-3af1d5752c1c](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2Frd0IihTwKZszWXYWgGpP%2Fimage.png?alt=media&token=8d058cd3-5150-434f-91db-3af1d5752c1c)

# **Adicionando dados.**

Diferente das [listas](https://solidity.web3dev.com.br/apostila/arrays-listas) onde indicamos o nome e a posição, com dicionários indicamos o nome e a chave. Nesse caso abaixo, dicionario balances no *endereço de quem chamar a transação* ([msg.sender](https://solidity.web3dev.com.br/apostila/variaveis-built-in-msg.sender-msg.value...)) terá o valor 100 guardado.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FkgWmtPtytvHAzzZ0uXCb%2Fimage.png?alt=media&token=06eb89af-dea4-4ec9-a7ae-0da92d62ee70](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FkgWmtPtytvHAzzZ0uXCb%2Fimage.png?alt=media&token=06eb89af-dea4-4ec9-a7ae-0da92d62ee70)

# **Ler dados.**

Também muito parecido com listas mas ao invés de passar a posição-da-lista onde estão os dados, passamos a chave que nesse caso também é aquele que chamar a transação.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FyIywocHcU4v8GXfAGy28%2Fimage.png?alt=media&token=901f028a-bd5a-4305-bfed-0c27b46cff37](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FyIywocHcU4v8GXfAGy28%2Fimage.png?alt=media&token=901f028a-bd5a-4305-bfed-0c27b46cff37)

acessar dados

# **Atualizar dados.**

Praticamente a mesma coisa que adicionar um novo dado, se no dicionário não existir nada no endereço de chave passado será adicionado pela primeira vez, se já existir algo será então substituído.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FBMMOSNq7Q0YPZICe8HmN%2Fimage.png?alt=media&token=e494340c-0c8a-475c-8dec-1e92aa14562a](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FBMMOSNq7Q0YPZICe8HmN%2Fimage.png?alt=media&token=e494340c-0c8a-475c-8dec-1e92aa14562a)

# **Deletar dados.**

Esse sim é exatamente como em listas, basta passar a chave do dicionário após a instrução ***delete***.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FVxDYQ5xG5Q5mS6MfonPR%2Fimage.png?alt=media&token=fc3bda3b-f489-46a8-bc7a-df8496d00330](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FVxDYQ5xG5Q5mS6MfonPR%2Fimage.png?alt=media&token=fc3bda3b-f489-46a8-bc7a-df8496d00330)

# **Valor padrão**

Listas e Dicionários tem um valor padrão caso tentemos acessar uma chave ou posição-de-lista que não exista, esse valor é 0.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FAtZamnLytemywyk9GPrq%2Fimage.png?alt=media&token=7d9c2fec-5638-49d6-a277-c316e1176b45](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FAtZamnLytemywyk9GPrq%2Fimage.png?alt=media&token=7d9c2fec-5638-49d6-a277-c316e1176b45)

# **Tipos Exóticos de Mappings.**

# **Dicionário de dicionários.**

É possível armazenar outros dicionários dentro de um dicionário. Imagine que você constrói um contrato em que é possível que outras pessoas guardem dinheiro e disponibilizem para outras pessoas além delas mesmas. Essa situação é representada no nosso exemplo abaixo onde temos um dicionario de endereços (chaves) principais (que guardam dinheiro no contrato) e os valores dentro desses endereços há outra lista de endereços que são chaves e dentro dessas chaves há valores bool, que podem ser positivo ou negativo.

Resumidamente, temos uma lista de endereços que guarda outros endereços e valors true ou false para indicar se esses endereços podem ou não realizar uma determinada ação.

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FB5WpsEqi0tyvOY87Nb14%2Fimage.png?alt=media&token=c5cd09af-3aef-40fa-b0f5-44e219c48cf0](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FB5WpsEqi0tyvOY87Nb14%2Fimage.png?alt=media&token=c5cd09af-3aef-40fa-b0f5-44e219c48cf0)

# **Listas dentro de dicionários**

Se estivermos contruíndo um jogo onde cada jogador pode jogar várias partidas e armazenar sua pontuação de cada partida para no final realizar um calcúlo.

Nesse caso, pode haver um dicionário que guarda endereços como chave e dentro de cada endereço há uma lista de valores.

# **14. Eventos**

Blockchains são sistemas isolados do resto da internet e sistemas convencionais e eventos são utilizados para "comunicar ao mundo" o que está acontecendo.

# **Declarando o Evento**

Possuem uma estrutura básica e padrão para que outros sistemas possam "falar todos a mesma lingua" e resumem-se à: quando, onde, quem e oque aconteceu. Para isso usamos a palavra chave e***vent*** antes do ***nomeDoEvento*** e entre parênteses os seus **argumentos obrigatórios**.

O parâmetro *indexed* permite que outros sistemas possam aplicar filtros, no exemplo abaixo um sistema que estiver *ouvindo* esses eventos poderá filtrar por data, endereço de envio e recebimento.

[]()

# **Emitindo o Evento**

Após declaramos um evento podemos emiti-lo dentro de qualquer função através do parâmetro ***emit nomeDoEvento()*** e então passamos os argumentos que são necessários.

[]()

# **Exemplo real: Transação.**

No exemplo abaixo um evento será emitido contendo *quem enviou*, *para quem enviou* e *quanto enviou*.

[]()

# **15. Modificadores**

São trechos de códigos que serão executados antes das funções. Uma das aplicações mais conhecidas é a de controle de acesso para que somente endereços específicos possam executar uma função.

# **Declarando um modifier**

No nosso exemplo vamos criar um modifier que irá verificar se o endereço que está chamando a função é o endereço que está salvo como administrador na variável *admin.* Se a instrução require retornar um true então será executado o código _; que significa: execute o que vem depois.

Isso quer dizer que se o código quebrar no require não irá executar a instrução *underline*, logo, não irá executar o código da função que vem depois.

[]()

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FLYVEbhFEpER6e6RlPEV6%2Fimage.png?alt=media&token=d2e3d415-d5e8-4984-b9c3-5616d30bd52d](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FLYVEbhFEpER6e6RlPEV6%2Fimage.png?alt=media&token=d2e3d415-d5e8-4984-b9c3-5616d30bd52d)

# **Passando parâmetros**

Para que modifiers possam receber parâmetros eles devem ser passados para as funções nas quais estão inseridos e ter seus nomes de variáveis idênticos.

[]()

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2F84sdJQLv1fWXdtu8u9LI%2Fimage.png?alt=media&token=d120cdb9-ddcf-40a1-9445-6f00309f2eb9](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2F84sdJQLv1fWXdtu8u9LI%2Fimage.png?alt=media&token=d120cdb9-ddcf-40a1-9445-6f00309f2eb9)

# **Combinando mais de um Modifier.**

É possível até mesmo encadear modifiers e passar dados entre eles, deve seguir a mesma nomenclatura para os parâmetros que serão passados.

[]()

![https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FUlnffndSEBLH6rhBwNow%2Fimage.png?alt=media&token=40a046ed-ac59-46e1-aea6-5555d03aed7a](https://3038272287-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FXT0NrtKBWFOa2UENeSLs%2Fuploads%2FUlnffndSEBLH6rhBwNow%2Fimage.png?alt=media&token=40a046ed-ac59-46e1-aea6-5555d03aed7a)

Modifiers são verificações então para ter mais de uma verificação/condição para que uma função possa ser executada basta inserir mais modifiers.