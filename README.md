# Ivanborisov
database:
  host: localhost
  port: 5432
  name: opendlp
  user: opendlp_user
  password: opendlp_password
targets:
  - type: mssql
    host: localhost
    port: 1433
    database: TestDLP
    username: SA
    password: 123qweR%
    tables:
      - Employees
    columns:
      - SSN
