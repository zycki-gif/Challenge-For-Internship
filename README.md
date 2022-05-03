# Challenge-For-Internship

Tabela Show - tabela contendo as informações com o nome do Show e a data
que o mesmo aconteceu. Os shows podem ser acessados pela rota
https://us-central1-raccoon-bi.cloudfunctions.net/psel_de_shows;
- Tabela Ingressos - tabela de vendas de ingressos da Amazing Tickets contendo a
pessoa, a data do show e o status da compra. As vendas podem ser acessadas
pela rota
https://us-central1-raccoon-bi.cloudfunctions.net/psel_de_ingressos;
- Tabela Compras - tabela contendo dados referentes a consumação das pessoas
e em quais shows. O consumo de cada pessoa pode ser acessado pela rota
https://us-central1-raccoon-bi.cloudfunctions.net/psel_de_compras.
Acesse e analise esses dados para responder a algumas perguntas:
1. Qual a média de gastos de pessoas com ingresso Pista?
2. Quais pessoas não compareceram aos shows?
3. Quais pessoas compraram ingressos com concorrentes?
4. Qual o dia com maior gasto?
5. Faça uma lista com os clientes que desistiram de comprar o ingresso com a AT, a
soma do valor que foi gasto durante os shows e quais shows eles desistiram de
comprar. Usar para resposta o esquema abaixo:
'''
{
"nome": <str>,
"gastos": <float>,
"shows": [<str>]
}
'''
Algumas considerações:
- A tabela Ingressos contém todas as tentativas de compra de ingresso com a
Amazing Tickets. Um cliente ainda pode ter comprado o ingresso com
concorrentes.
- A compra de um ingresso não significa que um cliente compareceu ao show.
- Todos os clientes que foram no show consumiram algo.
- Cada show ocorreu em um dia e não pode ter ocorrido mais de um show no
mesmo dia.
