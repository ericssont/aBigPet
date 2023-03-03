[M1S06] Ex 1 - Criar Entidades
Conforme o banco de dados criado nos exercícios do Módulo 1 - Semana 4. Vamos criar as classes que representam as tabelas deste banco de dados.
Abaixo, detalhes das tabelas do banco de dados:
A table Tutor deve conter ao menos 2 colunas: nome e idade;
A tabela Pet deve conter ao menos 4 colunas: nome, raça, tipo e tutor_id (chave estrangeira para a entidade Tutor e não obrigatório)
IMPORTANTE: Para a coluna "tutor_id" da classe Pet, é necessário utilizar uma relação "ManyToOne" com a classe Tutor.
Crie as classes que correspondem aos requisitos acima com seus mapeamentos (@Table, @Column, @Id, …).

[M1S06] Ex 2 - CRUD Tutor
Utilizando a injeção de dependência com classes de serviço e repositórios, crie API com endpoints para realizar todas as operações de CRUD (Create, Read, Update e Delete) para a entidade Tutor.

[M1S06] Ex 3 - CRUD Pet
Utilizando a injeção de dependência com classes de serviço e repositórios, crie API com endpoints para realizar todas as operações de CRUD (Create, Read, Update e Delete) para a entidade Pet.

[M1S06] Ex 4 - Consultar pets sem tutor
No Controller de Pets, crie um endpoint GET "/semtutor" que realize uma busca de todos os Pets que não tenham Tutor e retorne ordenando por nome ascendente (de A a Z).

[M1S06] Ex 5 - Adotar Pet
Como na classe Pet, o tutor não é obrigatório, crie um endpoint POST "/adotar" para que um Pet seja adotado por um Tutor. Nos parâmetros deste endpoint, será necessário ter ao menos o identificador (id) do Pet e o identificador (id) do Tutor.
