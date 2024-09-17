# sqlWorkshop1

1--Tedarikçi ID'si 1 ile 5 arasındaki ürünler--
SELECT * FROM Products
WHERE SupplierID BETWEEN 1 AND 5;

2--Tedarikçi ID'si 1, 2, 3, 4 veya 5 olan ürünler--
SELECT * FROM Products
WHERE SupplierID IN (1, 2, 4, 5);

3--Chang veya Aniseed Syrup olan ürünler--
SELECT * FROM Products
WHERE ProductName IN ('Chang', 'Aniseed Syrup');

4--Tedarikçi ID'si 3 olan veya birim fiyatı 10'dan büyük olan ürünler--
SELECT * FROM Products
WHERE SupplierID = 3 OR UnitPrice > 10;

5--Ürün adı ve birim fiyatı--
SELECT ProductName, UnitPrice FROM Products;

6--Büyük harfe dönüştürerek 'c' harfi içeren--
SELECT ProductName FROM Products 
WHERE UPPER(ProductName) LIKE '%C%';

7--'n' ile başlayan ve tek karakterli bir harf içeren--

8-- Stok miktarı 50den fazla olan ürünler--
SELECT * FROM Products
WHERE StockQuantity > 50;

9--En yüksek ve en düşük birim fiyatları--

10--Spice kelimesi geçen--
SELECT * FROM Products
WHERE ProductName LIKE '%Spice%';
