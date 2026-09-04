# Bank Transactions Analysis

A study project focused on working with a relational database containing information about bank clients, accounts, cards, and transactions.

## Project Overview

The project includes a relational database for storing information about bank clients, their accounts, cards, and financial transactions.

SQL queries were used to analyze the data, calculate key metrics, study transaction activity, and identify potentially anomalous transactions.

## Database Structure

The database consists of six tables:

`clients` — information about bank clients  
`types` — account types  
`categories` — purchase categories  
`accounts` — clients' bank accounts  
`cards` — bank cards linked to accounts  
`transactions` — financial transactions

The tables are connected using foreign keys.

## Analysis Performed

### Basic SQL Analysis

Calculated the total balance across all accounts for each client.

Analyzed the bank's total assets by currency.

Counted transactions for each purchase category.

Identified accounts with more than 5 transactions and calculated their average transaction amount.

Found the largest transaction for each client.

### Window Functions

Calculated the difference between the current and previous transaction for each account using `LAG()`.

Compared each transaction with the average transaction amount within its category.

Calculated the cumulative transaction history for each account using `SUM() OVER`.

### Anomaly Detection

A query was developed to identify transactions whose amount is more than twice the average transaction amount for the corresponding account.

This approach provides a simple example of identifying potentially unusual spending activity.

## SQL Techniques

`JOIN` · `GROUP BY` · `HAVING` · `SUM()` · `COUNT()` · `AVG()` · `MAX()` · `LAG()` · `SUM() OVER` · `COALESCE` · Subqueries

## Project Goal

The goal of the project is to practice SQL and develop skills in analyzing relational data, calculating analytical metrics, and identifying potentially anomalous transactions.
