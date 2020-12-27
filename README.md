# orcamentopessoal
 orcamentopessoal


###Cookes

utilizado o recurso web storage pois os navegadores modernos de forma geral implementam recursos de armazenamento de dados dentro do proprio navegador, antes do html 5 era usado o recurso de cookes mas com o advento do html 5  os browsers passaram a utilizar outros metodos para armazenamento local de dados, os cookes funcionam como dados que são armazenados do lado do cliente no browser e sempre que existe uma requisicao http ou seja, sempre que acessamos uma determnada pagina os cookies sao anexados a esta requisicao de tal modo que servidor tenha condicoes de acessar estas informacoes, extrair a sua logica de modo a entender as informaceos ja cadastradas no lado do cliente e apos este processamento fazer o retorno desta informacao requisitada pelo cliente, como nos sites de ecommerce que armazenam nossas consultas e nos retornam as consultas que fizemos, e isso é muito util pois fica armazenado do lado do cliente, e anexado na requisicao http, sendo permitido pelos servidores analisar requisicao por requisicao e retornar exatamente a logica de cada cliente.
o caso do local storage e session storage sao parecidos com os cookies com o diferencial de nao serem anexados a uma requisicao http e ficam de fato no navegador de modo analogo a uma aplicacao front-end, e pelo fato de nao terem que ser transmitidos por uma requisicao http permite que seja armazenado muito mais informacoes.
diferenca entre session storage e local storage

###session storage 
Armazena uma informacao enqualto o browser a instancia do navegador esta ativa, qyuando nos fechamos o navegador todas as informacoes mantidas nas instancias do navegador sao perdidas.

###local storage 
Podemos armazenar as informacoes fechar o as instancias do navegador, desligar a maquina ou reniciar a maquina e os dados iram persistir armazenados ate que ele seja intencionamente removidos.



###Notaçoes JSON

Armazenar os dados dentro de local storage, convertendo um objeto literal para JSON
tudo que vai dentro de uma string pode ser armazenado em um objeto mas no caso de uma notação tipo JSON esta string recebem algumas instruções como 
'{'categoria':'eletrodomestico'}'
mantendo chaves e valores encapisulados dentro das aspas intenamente também.


Recuperando um objeto literal previamente instanciado dentro da aplicação, e no processo de utlização deste objeto na função set item que vai abrir uma comunicação com o local storage, foi encaminhado um a representaçãco JSON deste objeto
        gravar(despesa)
}
function gravar(d){
    localStorage.setItem('despesa', JSON.stringify(d))
}
 de tal modo  que ao ser recuperado dentro da aplicação do outro lado no caso local storage a aplicação tenha a capacidade de fazer o parse desta informação convertendo em um novo objeto.

a instancia de um objeto existe apenas dentro de uma aplicação quando ela precisar se comunicar com um servidor ou com outras aplicações, no caso uma aplicação local storage é uma aplicão interna do browser mas uma aplicação externa a minha aplicação, consequentemente é necessario comunicaçao e para tal é necessario criar um protocolo de comunicação para que possam se comunicar os dados, porem objetos literais eles não podem ser transitados neste processo isso porque eles são objetos e estes objetos existem apenas na instancia da aplicação, logo nos precisamos de alguma forma transcrever este objeto em uma notação tipo testo no caso a notação JSON para que este texto nseja anexado a esta comunicação que pode ser feita tanto com a o back end ou com outras aplicações e o JSON atuara no entanto neste meio de campo de comunicação pois ele é suprtado nativamente pelo javascript.
Json é uma biblioteca inportante do javascript e a partir dela nos podemos utlizar o metodo strigfy que converte o projeto diretamente para um onjeto json sem a necessidade de ficar concatenando strings.
 o contrario também pode ser realizado tranformado um objeto JSCON em um objeto literal usando o metodo JSON.parse(produtoJSON)

 ###criação de indices dinamicos pra inclsuão de registro dentro de local storage

 recuperar os dados e inserir os dados no local storage, e agora é necessario gerar um novo registro conforme as criações forem feitas por isso necessario a criação de um indice dinamico, que ira incluir um novo intem sem sobrepor o indice anterior.


 ***Validação de dados 
 utilizando um componente do bootstrap chamado componente modal, ele exibe uma div na tela chamando a atenção do usuario para aquele respectivo ponto assim pondemos inserir as informaões que quero que o usuario se atente naquele momento em que ele esta digitando.
 
