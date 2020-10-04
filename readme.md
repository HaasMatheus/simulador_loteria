# Simulador

Este projeto é um simulador de *Mega-Sena*, onde o
usuário digite seis números.
E sorteamos aleatoriamente outros seis números e
quanto números você acertou.

**Não oficial**

##Tecnologias utilizadas
1. **HTML**: HTML é uma linguagem de marcação utilizada na construção de páginas na Web.
2. **CSS**: Cascading Style Sheets (CSS) é um mecanismo para adicionar estilo (cores, fontes, espaçamento, etc.) a um documento web
3. **JS**: JavaScript (frequentemente abreviado como JS) é uma linguagem de programação interpretada estruturada, de script em alto nível com tipagem dinâmica fraca e multiparadigma (protótipos, orientado a objeto, imperativo e, funcional)
4. ~**Jquery**~: Não foi utilizado(não sei por que colocar em tecnologias utilizadas então)

## Funções Principais
Aqui será apresentado as duas funções principais do site


### sorteio de números
Nessa função os números são sorteados aleatoriamente
```
function sortearNumeros() {
  numSort = [];
  let sort;
  for(var i = 0;i < 6 ;i++){
    do{
    sort = Math.ceil(Math.random() * 60);
    sort = (sort == 0) ? 1 : sort;
  }while (numSort.includes(sort))
      numSort.push(sort)
  }
}
```

###  Lendo os números digitados
Lê as entradas de números digitadas pelo usuário
```
function addToList(num, pos) {
  if(num.length == 2){
  if(numEsco.includes(num)){
    alert("Número escolhido anteriormente. Digite outro número")
  }else if(parseInt(num) > 60 ){
    alert("O n'umero digitado não pode ser maior que 60")
  }
  else{
    numEsco[pos-1] = num;
    }
  }
}
```
## Como Rodar o código
> Simplesmente baixe p código
e abra o arquivo **_index.html_** no seu navegador

## Exemplo de tabela
Alimentos | Preço
--------- | ------
Arroz     | R$ 10
Feijão    | R$ 8
Batata    | R$ 7
Macarrão  | R$ 8

## Imagens da tela
tela 1: tela de abertura
![tela 1](/imagens/tela1.png)
tela 1: 6 números digitados 1 sorteado  
![tela 1](/imagens/tela2.png)

## Referências
* HTML: [Wikipedia](https://pt.wikipedia.org/wiki/HTML)
* CSS: [Wikipedia](https://pt.wikipedia.org/wiki/CSS)
* JS: [Wikipedia](https://pt.wikipedia.org/wiki/JavaScript)
