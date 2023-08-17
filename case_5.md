SELECT nome, email, data_do_cadastro
FROM users_email
WHERE data_do_cadastro BETWEEN CURDATE() - INTERVAL 30 DAYS AND CURDATE();

// Utilizei o SELECT sem "*" para uma consulta mais específica, quero ver apenas o nome, email e a data em que efetuou o cadastro;
FROM foi utilziado para se referir a tabela users_email, visto que quero um chamado específico dessa tabela no meu banco de dados;
WHERE que define onde, a data de cadastro está entre (BETWEEN), CURDATE.
CURDATE refere-se á Current date, do inglễs que significa data atual.
INTERVAL 30 DAY define o periodo que estou subtraindo, que é dos 30 dias posteriores á data atual, garantindo que o resultado da consulta seja 30 dias atŕas.
Adiciono AND CURDATE() para incluir o dia atual que se equivale aos ultimos 30 dias
