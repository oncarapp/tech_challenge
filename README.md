# ONCar - Tech Challenge

A **ONCar** está em busca de pessoas incríveis que integrem nossa equipe para criarmos incríveis produtos digitais, e gostaríamos de ter você aqui conosco.

Para iniciar o processo, pedimos um teste que não vai tomar muito do seu tempo e nos dará uma perspectiva da sua forma de trabalhar. Queremos entender seu nível de habilidade em todas as áreas envolvidas na construção de um projeto: **Front e Back.**

Você não precisa entregar ambos, mas qualquer adicional as suas habilidades específicas é interessante.

# Requisitos do desafio

Crie uma aplicação que permitirá a gestão de veículos com suas determinadas caracteristicas como:
* Modelo
* Marca
* Cor

Além das informações adicionais que achar necessária;

Crie uma simulação para financiamento deste veículo, 
solicitando dados do cliente, gerando um SCORE de aprovação aleatório de 1 a 999 permitindo assim ele obter o carro 
com formas de pagamentos específicas.

Crie uma API Restful, que permitirá:

- Veículo
  - **GET**: Listará todos ou apenas um veículo
  - **POST**: Deve inserir uma nova solicitação de cartão.
  - **DELETE**: Remove uma solicitação

- Simulação
  - **POST**: Insere uma nova simulação para ser analisada

Quando o usuário inserir uma simulação, deve ter uma aprovação automática do sistema, que sua regra será:

Crie uma rotina que verificará a pontuação de crédito do usuário que será uma rotina que devolva uma pontuação **aleatória** entre 1 a 999, para ser utilizada como score de credito.

Por exemplo:

```
import random
random.randint(1, 999)
```

Sendo que, dependendo do score retornado a solicitação é aprovada ou não, também alterando o seu limite de crédito, que deverá seguir a seguinte lógica:

| Score     | Crédito                                        |
| --------- | ---------------------------------------------- |
| 1 a 299   | Reprovado                                      |
| 300 a 599 | 70% de entrada, 30% do comprometimento da renda|
| 600 a 799 | 50% de entrada, 25% do comprometimento da renda|
| 800 a 950 | 30% de entrada, 20% do comprometimento da renda|
| 951 a 999 | 100% de financiamento, taxa zero.              |

No Front, deverá ser listado todos os carros, com a possibilidade da inclusão de uma solicitação de crédito.

As rotas de alteração/deleção deverão ser expostas de alguma maneira, para serem utilizadas ou por um painel administrativo ou por ferramentas de requisições http (**POSTMAN**)

O **Back-End** do projeto deverá ser feito em **Python ou Node.JS**, utilizando um framework de sua escolha.

O **Front-End** deverá ser feito a seu critério e justificando o porque da solução escolhida, nós achamos o React interessante.



Qualquer dúvida sobre os requisitos, você pode enviar um e-mail para mateus.vieira@dmcard.com.br



# Como fazer?

Sugerimos um prazo de 7 dias para a entrega. Caso precise de mais nos avise e Justifique.

Sobre a entrega:

- **Pedimos que você nos envie um e-mail, para sinalizar seu início no desenvolvimento do desafio.**
- Seu código deve estar disponível em um repositório no Github.
- Você pode utilizar plataformas como Heroku ou AWS para nos mostrar a aplicação funcionando em produção.
- Quando estiver pronto nos envie o link do repositório.

Boa Sorte!
