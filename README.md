# code_challenge_dotnet

O objetivo deste teste é avaliar seus conhecimentos técnicos e domínio em .Net e C#, por isso deve ser feito por você. Você tem uma semana para entregar, se precisar de mais tempo entre em contato para nos informar. Leia as instruções com atenção!

## Descrição do projeto

O desafio consiste na criação de uma API para fazer CRUD de três entidades:
 - Contatos comerciais, que podem ser clientes ou fornecedores contendo os atributos:
    - Nome
    - tipo - cliente | fornecedor
    - Email - com validação de formato e unicidade no modelo
 - Propriedades produtivas, com os atributos:
    - Nome
    - Área
    - Espécie de planta
    - N° de plantas
    - Espaçamento entre fileiras 
      - Unidade de medida: centímetro ou metro.
    - Espaçamento entre plantas
      - Unidade de medida: centímetro ou metro.
 - Espécie de planta
    - Nome

### Informações: 
As entidades devem se relacionar da seguinte forma: Caso o contato comercial seja um fornecedor, pode ter até 3 propriedades. Clientes não têm nenhuma.

Ao excluir um fornecedor as propriedades pertencentes a ele devem ser excluídas também.

Uma propriedade pode ter N espécies de plantas e uma espécie de planta pode estar em N propriedades.      

O número de plantas deve ser calculado automaticamente utilizando o espaçamento entre fileiras e plantas com a fórmula: <b>nº de plantas = Área / (Espaçamento entre fileiras * Espaçamento entre plantas)</b>.

![Espaçamento entre filas e plantas](espaço-entre-plantas-.jpeg)

A API deve ter pelo menos os endpoints:
- CRUD Contatos comerciais
- CRUD Propriedades
- CRUD Espécie de planta

 

**Algumas observações:**

Ao retornar a lista deve-se exibir o nome dos contatos e ser ordenada pelo primeiro nome.

Na criação de uma propriedade não é obrigatório informar o número de plantas, mas ao retornar a lista de propriedades o número de plantas deve estar calculado de acordo com a fórmula apresentada acima.

Essas são as funcionalidades básicas que sua aplicação deve conter, sinta-se à vontade para adicionar recursos, se achar que faz sentido.

**Requisitos:**

- A aplicação deve ser implementada em .Net 6.0 e C#
- Deve utilizar apenas linguagens e bibliotecas livres ou gratuitas
- Os commits devem ser descritivos
- Utilize banco MySQL
- Testes são um grande diferencial
- Readme descrevendo o projeto e seu setup
- Disponibilize o Swagger para visualizar os recursos da API

## Instruções de entrega do desafio

1. Ao finalizar seu projeto crie um repositório no github
 - Se for privado dê acesso a @matheuscschenfeld
2. Envie via email o link do projeto para seu contato na Elysios com o título "[.Net dev] + seu nome"
3. Adicione ao readme uma breve descrição do que você fez e o passo a passo para subir a aplicação. 


# Avaliação

1. A aplicação deve conter as funcionalidades descritas e respeitar/atender as tecnologias requeridas;
2. Qualidade do seu código e estrutura do projeto;
3. As instruções de entrega devem ser seguidas conforme descrito bem como a apresentação do projeto no arquivo readme;
4. Qualidade e cobertura dos testes unitários.
5. O desafio deve ser entregue dentro do prazo de 7 dias.

---

Boa sorte!
