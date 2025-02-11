# dados-atletas

# Resumo do Projeto

Este projeto consiste em uma aplicação que recebe informações sobre atletas, calcula parâmetros relevantes e exibe os resultados para o usuário.

# Introdução

Os organizadores de uma competição solicitaram um software para avaliar atletas, incluindo suas notas, categoria, IMC e média válida das avaliações. A aplicação foi desenvolvida utilizando a linguagem JavaScript.

# Especificações

A aplicação utiliza uma classe Atleta para armazenar as informações e realizar os cálculos necessários. A classe possui os seguintes atributos:

nome: Nome do atleta.

idade: Idade do atleta.

peso: Peso do atleta.

altura: Altura do atleta.

notas: Notas atribuídas ao atleta.

A classe também conta com os seguintes métodos:

calculaCategoria(): Determina a categoria do atleta com base na idade.

calculaIMC(): Calcula o Índice de Massa Corporal (IMC) do atleta.

calculaMediaValida(): Calcula a média válida das notas, descartando a maior e a menor.

obtemNomeAtleta(): Retorna o nome do atleta.

obtemIdadeAtleta(): Retorna a idade do atleta.

obtemPesoAtleta(): Retorna o peso do atleta.

obtemNotasAtleta(): Retorna as notas do atleta.

obtemCategoria(): Retorna a categoria do atleta.

obtemIMC(): Retorna o IMC do atleta.

obtemMediaValida(): Retorna a média válida do atleta.

# Regras

Categoria do Atleta

Infantil: 9 a 11 anos

Juvenil: 12 a 13 anos

Intermediário: 14 a 15 anos

Adulto: 16 a 30 anos

Sem categoria: Outras idades

Cálculo do IMC

Fórmula: IMC = peso / (altura x altura)

Cálculo da Média Válida

A média é calculada com base nas três notas do meio, descartando a maior e a menor nota.

# Exemplo de Uso

const atleta = new Atleta("Cesar Abascal", 30, 80, 1.70, [10, 9.34, 8.42, 10, 7.88]);

console.log(`Nome: ${atleta.obtemNomeAtleta()}`);
console.log(`Idade: ${atleta.obtemIdadeAtleta()}`);
console.log(`Peso: ${atleta.obtemPesoAtleta()}`);
console.log(`Altura: ${atleta.altura}`);
console.log(`Notas: ${atleta.obtemNotasAtleta().join(",")}`);
console.log(`Categoria: ${atleta.obtemCategoria()}`);
console.log(`IMC: ${atleta.obtemIMC()}`);
console.log(`Média válida: ${atleta.obtemMediaValida()}`);

# Exemplo de Saída

Nome: Cesar Abascal
Idade: 30
Peso: 80
Altura: 1.7
Notas: 10,9.34,8.42,10,7.88
Categoria: Adulto
IMC: 27.68166089965398
Média válida: 9.25333333

# Tecnologias Utilizadas

JavaScript

# Autor

Desenvolvido por Danubio Medeiros Cabral

