# SQL-Semana2
Introdução ao SQL e Consultas Básicas
-- 1. Recuperar checkNumber, paymentDate e amount da tabela payments
SELECT checkNumber, paymentDate, amount
FROM payments;

-- 2. Recuperar orderDate, requiredDate e status dos pedidos com status 'Em Processamento', ordenados por orderDate decrescente
SELECT orderDate, requiredDate, status
FROM orders
WHERE status = 'Em Processamento'
ORDER BY orderDate DESC;

-- 3. Exibir firstName, lastName e email dos funcionários cujo cargo é 'Representante de vendas', ordenados por employeeNumber decrescente
SELECT firstName, lastName, email
FROM employees
WHERE jobTitle = 'Representante de vendas'
ORDER BY employeeNumber DESC;

-- 4. Recuperar todas as colunas e registros da tabela offices
SELECT *
FROM offices;

-- 5. Buscar productName e quantityInStock da tabela products, ordenados por buyPrice crescente, limitando a 5 registros
SELECT productName, quantityInStock
FROM products
ORDER BY buyPrice ASC
LIMIT 5;
