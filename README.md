# DIO - Trilha .NET - Fundamentos
www.dio.me

## Desafio de projeto
Para este desafio, você precisará usar seus conhecimentos adquiridos no módulo de fundamentos, da trilha .NET da DIO.

## Contexto
Você foi contratado para construir um sistema para um estacionamento, que será usado para gerenciar os veículos estacionados e realizar suas operações, como por exemplo adicionar um veículo, remover um veículo (e exibir o valor cobrado durante o período) e listar os veículos.

## Proposta
Você precisará construir uma classe chamada "Estacionamento", conforme o diagrama abaixo:
![Diagrama de classe estacionamento](diagrama_classe_estacionamento.png)

A classe contém três variáveis, sendo:

**precoInicial**: Tipo decimal. É o preço cobrado para deixar seu veículo estacionado.

**precoPorHora**: Tipo decimal. É o preço por hora que o veículo permanecer estacionado.

**veiculos**: É uma lista de string, representando uma coleção de veículos estacionados. Contém apenas a placa do veículo.

A classe contém três métodos, sendo:

**AdicionarVeiculo**: Método responsável por receber uma placa digitada pelo usuário e guardar na variável **veiculos**.

**RemoverVeiculo**: Método responsável por verificar se um determinado veículo está estacionado, e caso positivo, irá pedir a quantidade de horas que ele permaneceu no estacionamento. Após isso, realiza o seguinte cálculo: **precoInicial** * **precoPorHora**, exibindo para o usuário.

**ListarVeiculos**: Lista todos os veículos presentes atualmente no estacionamento. Caso não haja nenhum, exibir a mensagem "Não há veículos estacionados".

Por último, deverá ser feito um menu interativo com as seguintes ações implementadas:
1. Cadastrar veículo
2. Remover veículo
3. Listar veículos
4. Encerrar


## Solução
O código está pela metade, e você deverá dar continuidade obedecendo as regras descritas acima, para que no final, tenhamos um programa funcional. Procure pela palavra comentada "TODO" no código, em seguida, implemente conforme as regras acima.

Projeto Completo 

 Estrutura da Classe
A classe principal é Estacionamento, localizada no namespace:
Projeto_Estacionamento.Models
Ela contém:

Atributos privados

precoInicial — valor fixo cobrado na entrada
precoPorHora — valor multiplicado pelo número de horas
veiculos — lista de placas registradas

Construtor

Recebe o preço inicial e o preço por hora
Métodos públicos

AdicionarVeiculo()
RemoverVeiculo()
ListarVeiculos()

AdicionarVeiculo()
Solicita ao usuário uma placa e armazena na lista de veículos estacionados.

RemoverVeiculo()
Remove um veículo da lista, calcula o valor a pagar e exibe ao usuário.

Funcionalidades:

Verifica se a placa existe (ignorando maiúsculas/minúsculas)
Solicita a quantidade de horas
Calcula valorTotal = precoInicial + precoPorHora * horas
Remove a placa da lista
Informa o valor ao usuário

Exemplo:

Preço inicial: R$ 5,00
Preço por hora: R$ 2,00
Horas estacionado: 3