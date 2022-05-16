# Capítulo 1 - Dia 1 - Aprendendo os Conceitos de Blockchain

Olá! Sim sou eu. Seu desenvolvedor favorito de todos os tempos, Jacob. Você está visualizando o primeiro dia de todo o curso. Vamos começar essa jornada juntos.

Vamos começar nosso primeiro dia analisando o que parece ser termos complicados que você precisará entender para a jornada à frente.

## O que diabos é um Blockchain?

<img src="../../images/blockchain.png" alt="drawing" width="600"/>

*Se você já entende o que é o Blockchain ou simplesmente não se importa (isso é justo!), você pode pular esta seção.*

Ao aprender sobre o Blockchain, você pode encontrar alguns artigos complicados. É fácil ficar completamente perdido no molho e sentir vontade de desistir. Então, vou explicar o Blockchain de uma maneira muito fácil que pode ter algumas imprecisões/informações omitidas, mas destina-se a ajudá-lo a começar. **Especificamente, vou ajudá-lo a entender o Blockchain da perspectiva de alguém que está procurando codificar contratos inteligentes ou fazer alguns aplicativos descentralizados (os dois faremos!).**

Em uma frase: o Blockchain é um banco de dados aberto, descentralizado e compartilhado que permite que qualquer pessoa armazene coisas publicamente.

Ok, uau. O que isso significa?

1. **ABRIR**: Qualquer um pode interagir com ele. Não há restrições.
2. **DESCENTRALIZADO**: Ninguém o possui. Não há uma autoridade central ditando coisas.
3. **BASE DE DADOS**: Você pode armazenar informações sobre ele.
4. **PÚBLICO**: Qualquer pessoa pode visualizar os dados nele.

Por causa dessas coisas, podemos interagir com o Blockchain da maneira que quisermos. Muitas vezes, podemos querer configurar "livros de regras" que determinam como as pessoas podem interagir com partes específicas do Blockchain para que ele tenha alguma funcionalidade - especificamente nossos próprios aplicativos que definiremos. Isso é feito com contratos inteligentes.

Também é importante notar que existem muitos Blockchains diferentes por aí. Por exemplo, o Ethereum é provavelmente o Blockchain mais popular. Neste curso, aprenderemos sobre o maravilhoso Flow Blockchain, porque é aí que reside minha experiência ;)

## Contratos inteligentes? Ooo, isso soa legal.

<img src="../../images/smart contract.png" alt="drawing" width="600"/>

Por que sim, sim é. Contratos inteligentes são muito legais. Contratos inteligentes são programas ou "livros de regras" que os desenvolvedores fazem. Os desenvolvedores os criam porque nos permite especificar algumas funcionalidades com as quais os usuários podem interagir. Por exemplo, se eu quiser fazer um aplicativo que permita aos usuários armazenar suas frutas favoritas no Blockchain, preciso fazer um Contrato Inteligente que:

1. Tem uma função que qualquer um pode chamar
2. Leva em um parâmetro (a fruta favorita da pessoa)
3. Armazena esse parâmetro em alguns dados
4. Envia os dados atualizados para o Blockchain (acontece automaticamente)

Se eu criasse este Contrato Inteligente e o "implantasse" no Blockchain (implantado significa que colocamos o contrato no Blockchain para que as pessoas possam interagir com ele), qualquer um poderia colocar sua fruta favorita no Blockchain, e ele viveria lá para sempre e sempre! A menos que também tivéssemos uma função para remover esses dados.

Então, por que usamos contratos inteligentes?

1. **Velocidade, eficiência e precisão**: os contratos inteligentes são rápidos e não há intermediários. Também não há papelada. Se eu quiser atualizar os dados no Blockchain usando um Contrato Inteligente que me permita chamar alguma função, posso fazê-lo. Eu não tenho que obter a aprovação dos meus pais ou do meu banco.
2. **Confiança e transparência**: O Blockchain e, portanto, os Contratos Inteligentes, são extremamente seguros se os fizermos dessa maneira. É quase impossível hackear ou alterar o estado do Blockchain e, embora isso se deva a outros motivos, é em grande parte por causa dos contratos inteligentes. Se um Contrato Inteligente não me permite fazer algo, simplesmente não consigo. Não há maneira de contornar isso.

Quais são algumas desvantagens?
1. **Difícil de acertar**: Embora os contratos inteligentes sejam legais, eles NÃO são inteligentes. Eles exigem níveis sofisticados de conhecimento do lado do desenvolvedor para garantir que não tenham problemas de segurança, são baratos e fazem o que queremos que façam. Vamos aprender tudo isso mais tarde.


3. **Pode ser mal-intencionado se o desenvolvedor for malvado**: Se um desenvolvedor quiser fazer um Contrato Inteligente que roube seu dinheiro e, em seguida, induza você a chamar uma função que faz isso, seu dinheiro será roubado. No mundo do Blockchain, você deve se certificar de interagir com Smart Contracts que você sabe que são seguros.
4. **Não é possível desfazer algo**: Você não pode simplesmente desfazer algo. A menos que você tenha uma função que permita.

## Transações e scripts

<img src="../../images/transaction.jpeg" alt="drawing" width="600"/>

*"Ok, então nós temos um Contrato Inteligente. Como eu realmente interajo com ele? Você continua dizendo para chamar uma função, mas o que isso significa!?"*

**Uma transação é uma chamada de função glorificada e paga.** Essa é a forma mais simples que posso colocar. O que é importante saber é que uma transação MUDA os dados no Blockchain, e geralmente é a ÚNICA maneira que podemos alterar os dados no Blockchain. As transações podem custar diferentes quantias de dinheiro, dependendo de qual Blockchain você está. No Ethereum, para armazenar sua fruta favorita no Blockchain, pode custar quase 100 $. No Flow, são frações de centavo.

Por outro lado, um script é usado para VISUALIZAR dados no Blockchain, eles não o alteram. Scripts não custam dinheiro, isso seria ridículo.
Aqui está o fluxo de trabalho normal:
1. Um desenvolvedor "implanta" um contrato inteligente no Blockchain
2. Um usuário executa uma "transação" que recebe algum pagamento (para pagar taxas de gás, execução, etc.) que chama algumas funções no Contrato Inteligente
3. **O contrato inteligente altera seus dados de alguma forma**

## "MainNet" vs. "TestNet"

<img src="../../images/tvm.PNG" alt="desenho" largura="600"/>

Você pode ter ouvido esses termos surgirem, mas o que eles realmente significam?

**TestNet** é um ambiente onde os desenvolvedores testam seus aplicativos antes de lançá-los ao público. Este é um espaço perfeito para descobrir o que há de errado com seu aplicativo antes de liberá-lo para uso público. Aqui estão algumas notas adicionais:

- Tudo é falso
- Nenhum dinheiro real envolvido
- As transações custam dinheiro falso
- Uma boa maneira para os desenvolvedores testarem seus contratos e aplicativos inteligentes ANTES de lançar ao público
- Se algo ruim acontecer, ninguém se importa.

**MainNet** é um ambiente onde tudo é real. Quando você libera seu aplicativo para o público, você o coloca na MainNet. Na MainNet, tudo é ao vivo, então as coisas custam dinheiro real, existem riscos e você deve garantir que tudo esteja funcionando corretamente. Aqui estão algumas notas adicionais:
- Tudo é real
- O dinheiro está envolvido
- As transações custam dinheiro real
- Quando seu aplicativo estiver totalmente pronto, você o coloca na MainNet para que os usuários possam interagir.
- Se algo ruim acontecer, isso é muito ruim.

## Aplicativos Descentralizados (DApps)

<img src="../../images/dapps.jpeg" alt="drawing" width="300"/>

Oh não, isso parece complicado. Não! Não é. DApps são literalmente apenas aplicativos normais (Javascript, Python, etc) que TAMBÉM têm contratos inteligentes envolvidos. É isso.

Além disso, estaremos construindo estes :)

## Por que eu me importo com tudo isso?

Bem, porque é disso que se trata este curso, idiota! Neste curso, faremos nossos próprios contratos inteligentes, especificamente no Flow Blockchain. Além disso, faremos aplicativos descentralizados que *usam* esses contratos inteligentes.
## Conclusão

Jacó é o melhor. Não não. Essa não é a conclusão. A conclusão é que, embora tudo isso pareça muito complicado, na verdade não é. E se você ainda não entende NADA disso, tudo bem. Às vezes é melhor pular para alguns exemplos para fazer as coisas fazerem mais sentido. Faremos isso nos próximos dias.

# missões

Você é livre para responder a essas perguntas em seu próprio idioma de escolha. E não, não me refiro a linguagem de programação de computador, haha.

1. Explique o que é Blockchain com suas próprias palavras. Você pode ler isso para ajudá-lo, mas você não precisa:
https://www.investopedia.com/terms/b/blockchain.asp

2. Explique o que é um Contrato Inteligente. Você pode ler isso para ajudá-lo, mas você não precisa: https://www.ibm.com/topics/smart-contracts

3. Explique a diferença entre um script e uma transação.
