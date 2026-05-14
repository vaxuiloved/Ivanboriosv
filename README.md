# Ivanborisov
database:
  host: localhost
  port: 5432
  name: ivan
  user: user
  password: opendlp_password

targets:
  - type: mssql
    host: localhost
    port: 1433
    database: TestDLP
    username: ivan
    password: 123qweR%
    tables:
      - Employees
    columns:
      - SSN
