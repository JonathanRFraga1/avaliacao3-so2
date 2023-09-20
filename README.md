# Trabalho Avaliativo - Sistemas Operacionais II (SO II)

O enunciado apresentado a seguir corresponde a um trabalho avaliativo da primeira etapa da disciplina de Sistemas Operacionais II (SO II). Refere-se à realização da avaliação prática sobre Problemas de Programação Concorrente, cujos objetivos são:

- [x] Associar os paradigmas e problemas de programação concorrente com o escopo de Sistemas Operacionais.
- [x] Implementar o algoritmo utilizando a Linguagem de Programação Java.
- [x] Implementar esse problema utilizando monitores/semáforos.

## Descrição do Problema

Imagine um supermercado com várias prateleiras de produtos. Os clientes compram produtos das prateleiras e esses produtos precisam ser repostos quando o estoque estiver baixo. Para resolver esse problema, você pode criar um sistema de gerenciamento de estoque que utiliza threads para coordenar as seguintes tarefas:

a) Cada cliente é representado por uma thread. Quando um cliente seleciona um produto e o coloca no carrinho, a quantidade desse produto no estoque deve ser reduzida de forma segura para evitar que dois clientes comprem o mesmo produto ao mesmo tempo.

b) Thread de Reposição de Estoque: Uma ou mais threads são responsáveis por repor o estoque quando um produto fica com um nível baixo. Essas threads monitoram constantemente o nível de estoque de cada produto e reabastecem as prateleiras conforme necessário. A sincronização é crucial aqui para evitar que várias threads de reposição acessem o mesmo produto simultaneamente.

c) Thread de Verificação de Estoque: Uma thread adicional pode ser responsável por verificar regularmente os níveis de estoque de todos os produtos e gerar alertas quando o estoque estiver muito baixo ou quando os produtos estiverem prestes a expirar (no caso de produtos perecíveis).

## Regras

- [x] O trabalho poderá ser realizado em grupos de no máximo dois integrantes.
- [x] Cópias integrais ou parciais de colegas e/ou da Internet receberão nota ZERO.

## Primeiros Passos

- [] Fazer UM cliente para comprar valores aleatórios de um ÚNICO produto
 
- [] Fazer UM produto com um estoque de 30, quando está abaixo de 15, o estoque é renovado (Pode ser renovado de forma sync)

3 Threads - Cliente, repositor de estoque e verifica estoque