# Binary Search Tree Projesi
## Veri Yapıları ve Algoritmalar eğitiminin üçüncü ödevi.

### [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

1. Aşama sonucu: 

- İkili arama ağacı, her düğümün solundaki koldan ulaşılabilecek bütün verilerin düğümün değerinden küçük, sağ kolundan ulaşılabilecek verilerin değerinin o düğümün değerinden büyük olmasını şart koşar.

|Açıklama   |   |   |   |
|---|---|---|---|
|root=7     |   |7  |  |
---
2. Aşama sonucu:

- 5 değeri 7 değerinden küçük olduğundan sol tarafa yazılır.

|Açıklama   |   |   |   |
|---|---|---|---|
|   |   |   |7  |
|   |   | /  |   |
|5 eklendi  | 5  |   |   |
---
3. Aşama sonucu:

- 1 sayısı 5'ten ve 7'den küçük olduğundan sol tarafa yazılır.

|Açıklama   |   |   |   |   |   |
|---|---|---|---|---|---|
|   |   |   |   |   | 7  |
|   |   |   |   | /  |   |
|   |   |   | 5  |   |   |
|   |   | /  |   |   |   |
|1 eklendi   | 1  |   |   |   |   |
---
4. Aşama sonucu:

- 8 sayısı 7'den büyük olduğundan sağına ekledik.

|Açıklama   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|
|   |   |   |   |   | 7  |   |   |
|   |   |   |   | /  |   | \  |   |
|8 eklendi   |   |   | 5  |   |   |   | 8 |
|   |   | /  |   |   |   |   |   |
|   | 1  |   |   |   |   |   |   |
---
5. Aşama sonucu:

- 3 sayısı 7'den ve 5'ten küçük olduğunda 5'in soluna, 1'den büyük olduğunda 1'in sağına ekledik.

|Açıklama   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|
|   |   |   |   |   | 7  |   |   |
|   |   |   |   | /  |   | \  |   |
|   |   |   | 5  |   |   |   | 8  |
|   |   | /  |   | \  |   |   |   |
|   | 1  |   |   |   | 6  |   |   |
|   |   | \  |   |   |   |   |   |
|3 eklendi   |   |   | 3  |   |   |   |   |
---
6. Aşama sonucu:

- 0 sayısı 7'den, 5'ten ve 1'den küçük olduğunda 1'in soluna ekledik.

|Açıklama   |   |   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   | 7  |   |   |
|   |   |   |   |   |   | /  |   | \  |   |
|   |   |   |   |   | 5  |   |   |   | 8 |
|   |   |   |   | /  |   | \  |   |   |   |
|6 eklendi   |   |   | 1  |   |   |   | 6 |   |   |
|   |   | /  |   | \  |   |   |   |   |   |
|   | 0  |   |   |   | 3  |   |   |   |   |
---
7. Aşama sonucu:

- 0 sayısı 7'den, 5'ten ve 1'den küçük olduğunda 1'in soluna ekledik.

|Açıklama   |   |   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   | 7  |   |   |
|   |   |   |   |   |   | /  |   | \  |   |
|   |   |   |   |   | 5  |   |   |   | 8 |
|   |   |   |   | /  |   | \  |   |   |   |
|   |   |   | 1  |   |   |   | 6 |   |   |
|   |   | /  |   | \  |   |   |   |   |   |
| 0 eklendi  | 0  |   |   |   | 3  |   |   |   |   |
---
8. Aşama sonucu:

- 9 sayısı 7'den ve 8'den büyük olduğunda 8'in sağına ekledik

|Açıklama   |   |   |   |   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   | 7  |   |   |   |   |
|   |   |   |   |   |   | /  |   | \  |   |   |   |
|   |   |   |   |   | 5  |   |   |   | 8 |   |   |
|   |   |   |   | /  |   | \  |   |   |   | \  |   |
| 9 eklendi  |   |   | 1  |   | 6  |   |   |   | 9  |
|   |   | /  |   | \  |   |   |   |   |   |   |   |
|   | 0  |   |   |   | 3  |   |   |   |   |   |   |
---
9. Aşama sonucu:

- 4 sayısı 7'den ve 5'ten küçük olduğunda 5'in soluna, 1'den ve 3'ten büyük olduğunda 3'ün sağına ekledik.

|Açıklama   |   |   |   |   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   | 7  |   |   |   |   |
|   |   |   |   |   |   | /  |   | \  |   |   |   |
|   |   |   |   |   | 5  |   |   |   | 8  |   |   |
|   |   |   |   | /  |   | \  |   |   |   | \  |   |
|   |   |   | 1  |   |   |   | 6  |   |   |   | 9  |
|   |   | /  |   | \  |   |   |   |   |   |   |   |
|   | 0  |   |   |   | 3  |   |   |   |   |   |   |
|   |   |   |   |   |   | \  |   |   |   |   |   |
|4 eklendi   |   |   |   |   |   |   | 4  |   |   |   |   |
---
10. Aşama sonucu:

- 2 sayısı 7'den ve 5'ten küçük olduğunda 5'in soluna, 1'den büyük olduğunda 1'in sağına ve 3'ten küçük olduğunda 3'ün soluna ekledik.

|Açıklama   |   |   |   |   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   | 7  |   |   |   |   |
|   |   |   |   |   |   | /  |   | \  |   |   |   |
|   |   |   |   |   | 5  |   |   |   | 8  |   |   |
|   |   |   |   | /  |   |   |   |   |   | \  |   |
|   |   |   | 1  |   |   |   |   |   |   |   | 9  |
|   |   | /  |   | \   |   |   |   |   |   |   |   |
|   | 0  |   |   |   | 3  |   |   |   |   |   |   |
|   |   |   |   | /  |   | \   |   |   |   |   |   |
|2 eklendi   |   |   | 2  |   |   |   | 4  |   |   |   |   |