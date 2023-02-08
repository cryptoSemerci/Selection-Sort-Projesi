# Selection Sort Projesi

[22,27,16,2,18,6] -> Insertion Sort

  1. [22,**27**,16,2,18,6] -> 1. Adım: 0. index (22) ile 1. index (27) karşılaştırılır, 22 zaten küçük olduğundan yer değiştirilmez -> [22,**27**,16,2,18,6]
  2. [22,27,**16**,2,18,6] -> 2. Adım: 1. index (27) ile 2. index (16) karşılaştırılır, 16 küçük olduğundan yer değiştirilir, ardından 0. index (22) ile 1. index (16) tekrar karşılaştırılır, yine 16 küçük olduğundan yer değiştirilirler -> [**16**,22,27,2,18,6]
  3. [16,22,27,**2**,18,6] -> 3. Adım: 2. index (27) ile 3. index (2) karşılaştırılır, 2 küçük olduğundan yer değiştirirler, ardından 2 sayısı sırasıyla 1. ve 0. indexlerle karşılaştırılır, hepsinden küçük olduğu için en başa koyulur. -> [**2**,16,22,27,18,6]
  4. [2,16,22,27,**18**,6] -> 4. Adım: 3. index (27) ile 4. index (18) karşılaştırılır, 18 küçük olduğundan yer değiştirilirler, ardından sırasıyla 2. ve 1. indexlerle karşılaştırılır, 2. indexten küçük olduğu için yer değiştirir fakat 1. indexten büyük olduğu için bir daha değişim olmaz ve adım biter. -> [2,16,**18**,22,27,6]
  5. [2,16,18,22,27,**6**] -> 5. Adım: 4. index (27) ile 5. index (6) karşılaştırılır, 6 küçük olduğundan yer değiştirirler, ardından sırasıyla 3., 2., 1. ve 0. indexler ile karşılaştırılır, 6 sayısı 3., 2. ve 1. indexten küçük olduğu için sırasıyla yer değiştirme işlemleri yapılır, fakat 0. indexten büyük olduğu için yer değiştirme yapılmaz, adım biter. -> [2,**6**,16,18,22,27] -> Son indexe kadar tarama yapaıldığı için Sorting işlemi tamamlanmıştır.

Big-O(n^2)

[7,3,5,8,2,9,4,15,6] -> Selection Sort

  1. [7,3,5,8,2,9,4,15,6] -> 1. Adım: En küçük sayı (2) bulunur (4. index) ve 0. index (7) ile yer değiştirilir. -> [**2**,3,5,8,**7**,9,4,15,6]
  2. [2,3,5,8,7,9,4,15,6] -> 2. Adım: 0. index yok sayılıp en küçük sayı (3) bulunur (1. index), zaten 1. indexte olduğu için işlem yapılmaz. -> [2,**3**,5,8,7,9,4,15,6]
  3. [2,3,5,8,7,9,4,15,6] -> 3. Adım: İlk 2 index yok sayılıp en küçük sayı (4) bulunur (6. index) ve 2. index (5) ile yer değiştirilir. -> [2,3,**4**,8,7,9,**5**,15,6]
  4. [2,3,4,8,7,9,5,15,6] -> 4. Adım: İlk 3 index yok sayılıp en küçük sayı (5) bulunur (6. index) ve 3. index (8) ile yer değiştirilir. -> [2,3,4,**5**,7,9,**8**,15,6]
