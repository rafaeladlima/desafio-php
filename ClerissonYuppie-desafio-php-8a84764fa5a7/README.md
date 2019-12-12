# Desafio PHP #

Olá, bem vindo ao nosso desafio para vaga de Desenvolvedor PHP.
Crie um respositório privado em seu Bitbucket e adicionar o email: clerisson@yuppietech.com.br

### Requisitos! ###

* PHP 7.1 (Zend 1 / Laravel)
* MySql 5.6

### O que precisa ser feito? ###

* CRUD de Produtos. Precisamos também de uma funcionalidade que importe produtos de um arquivo .csv, alimente a tabela de produtos e turmas_materiais
* CRUD de Alunos. As informações de endereço devem ser consultadas da API (viacep.com.br)
* Tela para vendas de materiais.

### Tabelas ###

Alunos          | Tipo
----------------| ------
id              | Numérico
nome            | Texto
data_nascimento | Data
turma_id        | Numérico
cep             | Numérico
endereco        | Texto
bairro          | Texto
cidade          | Texto
uf              | Texto

Produtos | Tipo
---------| ------
id       | Numérico
nome     | Texto
estoque  | Numérico
preco    | Monetário

Turmas | Tipo
------ | ------
id     | Numérico
nome   | Texto

Turmas Materiais | Tipo
---------------- | ------
id               | Numérico
turma_id         | Numérico
produto_id       | Numérico

Vendas     | Tipo
-----------| ------
id         | Numérico
aluno_id   | Numérico
data       | Data
finalizada | Condicional

Vendas Itens | Tipo
------------ | ------
id           | Numérico
venda_id     | Numérico
produto_id   | Data
preco        | Monetário
quantidade   | Numérico

### Funcionalidades ###
* Atenção, os itens vendidos para o aluno devem ter relação com a tabela turmas_materiais.
* Quando a venda for finalizada o produto deve ser debitado do estoque, não precisamos de informações de pagamento.
* O arquivo .csv está neste repositorio

Boa sorte!