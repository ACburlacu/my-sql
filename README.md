## 1. Create (INSERT)
### a. Add a new product
```
INSERT INTO product
VALUES (NULL, "Product", 999)
```
![Screenshot 2025-03-12 124730](https://github.com/user-attachments/assets/0b2fad9c-4782-4c8c-9396-c783472c3f48)

### b. Add a new address for user with ID of 3
```
INSERT INTO address
VALUES (NULL, 3, "Address", "City")
```
![Screenshot 2025-03-12 124638](https://github.com/user-attachments/assets/c39e6893-13b3-42a1-8b19-020d6229b8e1)

## 2. Read (SELECT)
### a. Select everything
```
SELECT * FROM product
```
![Screenshot 2025-03-12 125151](https://github.com/user-attachments/assets/3f62e072-a03f-4f15-b251-e0babe904157)

### b. Select everything priced between 100 and 500
```
SELECT * FROM product
WHERE ProductPrice > 100 AND ProductPrice < 500
```
![Screenshot 2025-03-12 125425](https://github.com/user-attachments/assets/62201001-7da1-4d16-a908-90fe4de9cd75)

### c. Select every customer whose name starts with "P"
```
SELECT * FROM customer
WHERE CustomerName LIKE "P%"
```
![Screenshot 2025-03-12 125717](https://github.com/user-attachments/assets/f1e1ee10-feeb-4507-8e94-c4a9dde1a8ad)

### d. Order every customer in alphabetical order
```
SELECT * FROM customer
ORDER BY CustomerName ASC
```
![Screenshot 2025-03-12 125926](https://github.com/user-attachments/assets/c6e5a194-023b-4d9b-8e4f-dc43b0d57cf7)

### e. Select the first four addresses
```
SELECT * FROM address LIMIT 4
```
![Screenshot 2025-03-12 130106](https://github.com/user-attachments/assets/c88da151-c279-423c-abd1-f2a1d1cfa314)

## 3. Update (UPDATE)
### a. Edit a single price tag
```
UPDATE product SET ProductPrice = 15
WHERE ProductID = 3
```
![Screenshot 2025-03-12 132829](https://github.com/user-attachments/assets/611139a0-9d3b-4e45-94e9-283f5f244762)

### b. Modify city of customer with ID of 1 to "Iasi"
```
UPDATE address SET AddressCity = "Iasi"
WHERE CustomerID = 1
```
![image](https://github.com/user-attachments/assets/e1784666-b881-473c-a4b2-ef64c52996e4)
