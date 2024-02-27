# Atividade-SQL
Atividade de SQL no geral consegui realizar mas tive algumas dificuldades principalmente na primeira questão que tive que primeiro tive que achar o total de usuarios para depois achar o de produtos.

Segue as respostas
  1- Consulta com o numero de registros na tabela

SELECT COUNT(*)
AS total_registros USUARIOS;
16

SELECT COUNT(*)
AS total_registros PRODUTOS ;
15

  2- Consulta para encontrar o usuario com o id 10

SELECT *
FROM USUARIOS WHERE id = 10;
10 LUCCA RYAN JESUS

  3- Consulta para encontrar o nome do Bruce Wayne

FROM Usuario WHERE nome = 'Bruce Wayne';

13 brucewayne@gothan.com


  4- Consulta para encontrar o email do usuario 'ghost_silva@fantasma.com'

SELECT FROM USUARIOS WHERE email = 'ghost_silva@fantasma.com';

4 Ghost Silva ghost_silva@fantasma.com

  5- Realizar uma consulta para deletar o usuario 'peterparker@marvel.com'

DELETE FROM USUARIOS WHERE email = 'peterparker@marvel.com';

  Produtos

  1- Produtos com descrição vazia

SELECT * FROM Produtos WHERE DESCRICAO = '';

5 caneca chopp         utilitários        R$25,5

6 copo grande térmico  utilitários        R$35,9

  2- Produtos na categoria games

SELECT * FROM Produtos WHERE categoria = 'games';

7   MOUSE GAMER         GAMES   R$101,00    MOUSE COM LEDS

8   TECLADO GAMER       GAMES   R$99,00     TECLADO COM LEDS

9   MONITOR GAMMER      GAMES   R$1500,00   MONITOR GRANDE PRA JOGAR

10  JOGO BATMAN         GAMES   R$150      JOGO BATMAN PARA PC

11  JOGO TOMB RAIDER    GAMES   R$100      JOGO TOMB RAIDER GAMES PARA PC

12  JOGO SPIDER-MAN     GAMES   R$200      JOGO SPIDER-MAN PARA PC

3- Produtos com o preço 0

SELECT * FROM Produtos WHERE preco = 0;

3 adesivo  utilitários R$0,00   adesivo com precificação

4 caneca   utilitários R$0,00   caneca para café

4- Produtos com o preço maior que 100

SELECT * FROM Produtos WHERE preco > 100.00;

7   mouse gamer     games   R$101,00    mouse com leds.

9   monitor         games   R$1500,00   monitor grande para jogar.

10  jogo batman     games   R$150,00    jodo do batman para pc.

12  jogo spider-man games   R$200,00    jogo spider-man para pc.

13  jogo pac-man    games   R$180,00    jogo pac-man para xb.

14  guarda-roupas   casa    R$2500,00   guarda-roupas gigante.

15  cama solteiro   casa    R$1800,00   cama box solteiro.

  5- Produtos com os preços entre 1000 e 2000.

SELECT * FROM Produtos WHERE preco BETWEEN 1000.00 AND 2000.00;

9   minitor gamer   games  R$1500,00    monitor grande para jogar.

15  cama solteiro   casa   R$1800,00    cama box solteiro.

  6- Produtos que tenha a palavra jogo

SELECT * FROM Produtos WHERE nome LIKE '%jogo%';
10 jogo batman games      R$150,00  jogo do batman para PC.

11 jogo tomb raider games R$100,00  jogo tomb raider para PC.

12 jogo spider-man games  R$200,00  jogo spider-man  para PC.

13 JOGO pac-man games     R$180,00  jogo pac-man para Xb.
