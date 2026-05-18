# RPCW2026 - Normal

## Identificação

Nome: Rodrigo Sousa  
Número: PG60302  

## Descrição

Este repositório contém a resolução do teste normal de RPCW2026.

Foram desenvolvidas ontologias OWL em formato Turtle, usando o Protégé, e foram criadas queries SPARQL para testar o conhecimento representado no GraphDB.

## Exercício 1 - Fábula

Neste exercício foi criada uma ontologia para representar o conhecimento presente na fábula do Corvo e da Raposa.

A ontologia inclui classes como Personagem, Animal, Objeto, Local, Sentimento e Característica.  
Foram também criadas relações entre indivíduos, como posse, localização, interação, engano e características associadas às personagens.

Ficheiros:

- `fabula.ttl`
- `queries.txt`

## Exercício 2 - Jogos de Tabuleiro

Neste exercício foi criada uma ontologia sobre jogos de tabuleiro modernos.

A ontologia base define as classes principais, as data properties e as object properties necessárias para representar jogos, autores, editoras, mecânicas, prémios e categorias.

Depois, a ontologia foi povoada com indivíduos retirados dos ficheiros JSON fornecidos no enunciado.

Ficheiros:

- `boardgames_base.ttl`
- `boardgames_ind.ttl`
- `sparql.txt`

## Como foi feito

A modelação da ontologia foi feita no Protégé.

Primeiro foram criadas as classes principais.  
De seguida foram definidas as data properties para representar atributos literais, como nome, país, ano, número de jogadores e duração do jogo.  
Depois foram definidas as object properties para representar relações entre indivíduos, como autores de jogos, editoras, mecânicas utilizadas, prémios ganhos e categorias.

O povoamento da ontologia foi feito através da criação de indivíduos correspondentes aos dados presentes nos ficheiros JSON.

As queries SPARQL foram testadas no GraphDB, após importar os ficheiros `.ttl`.

## Execução no GraphDB

Para testar as queries:

1. Abrir o GraphDB.
2. Criar um repositório.
3. Importar o ficheiro `.ttl` correspondente.
4. Abrir o separador SPARQL.
5. Executar as queries presentes nos ficheiros `queries.txt` e `sparql.txt`.

## Ficheiros entregues

- `fabula.ttl`
- `queries.txt`
- `boardgames_base.ttl`
- `boardgames_ind.ttl`
- `sparql.txt`
- `README.md`
