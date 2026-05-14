# Ivanborisov
-- Создание базы данных
CREATE DATABASE TestDLP;
GO

-- Переход в созданную БД
USE TestDLP;
GO

-- Создание таблицы с конфиденциальными данными
CREATE TABLE Employees (
    ID INT PRIMARY KEY,
    Name NVARCHAR(100),
    Salary DECIMAL(10, 2),
    SSN NVARCHAR(20)  -- Поле с персональными данными (номер SSN)
);
GO

-- Заполнение тестовыми данными
INSERT INTO Employees VALUES
(1, 'Иван Иванов', 50000, '123-45-6789'),
(2, 'Мария Петрова', 60000, '987-65-4321'),
(3, 'Алексей Сидоров', 55000, '555-12-3456');
GO

-- Проверка данных
SELECT * FROM Employees;
GO
