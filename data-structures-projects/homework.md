# Data Structures & Algorithms Projects

# Project 1 - Selection Sort Projesi

[22, 27, 16, 2, 18, 6] -> Insertion Sort

Yukarıda gösterilen dizinin sort türüne göre aşamalarını yazın. Big-O gösterimini yazın.

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case' lerden hangisinin kapsamına girer yazınız.

1) Average Case: Aradığımız sayının ortada olması
2) Worst Case: Aradığımız sayının sonda olması
3) Best Case: Aradığımız sayının en başlarda olması

- [7, 3, 5, 8, 2, 9, 4, 15, 6] dizisinin Selection Sort' a göre ilk dört adımını yazınız:

### Solution:

[22] Başlangıçta sadece bir eleman sıralı kabul edilir.
[22, 27] 27, 22'den büyük olduğu için sıraya eklenir.
[16, 22, 27] 16, 22'den küçük olduğu için 22 ve 27'nin önüne eklenir.
[2, 16, 22, 27] 2, 16'dan küçük olduğu için 16, 22 ve 27'nin önüne eklenir.
[2, 16, 18, 22, 27] 18, 16'dan büyük, 22 ve 27'den küçük olduğu için araya eklenir.
[2, 6, 16, 18, 22, 27] 6, 2'den büyük, 16, 18, 22 ve 27'den küçük olduğu için sıraya eklenir.

## Big-O Notation:

Big-O gösterimi: O(n^2) - En kötü durumda, tüm elemanlar diziyi taranır ve yerlerine yerleştirilir.

## Time Complexity:

[2, 6, 16, 18, 22, 27] ->  Dizi sıralandıktan sonra 18 sayısı "Average case" kapsamına girer.

## Selection Sort:

Verilen dizi: [7, 3, 5, 8, 2, 9, 4, 15, 6],
Sıralama aşamaları:

[2, 3, 5, 8, 7, 9, 4, 15, 6] (Minimum elemanı 2 olduğu için ilk eleman ile değiştirilir)
[2, 3, 4, 8, 7, 9, 5, 15, 6] (Minimum elemanı 4 olduğu için ikinci eleman ile değiştirilir)
[2, 3, 4, 5, 7, 9, 8, 15, 6] (Minimum elemanı 5 olduğu için üçüncü eleman ile değiştirilir)
[2, 3, 4, 5, 6, 9, 8, 15, 7] (Minimum elemanı 6 olduğu için dördüncü eleman ile değiştirilir)

*****************************************************************

# Project 2 - Merge Sort Projesi

[16,21,11,8,12,22] -> Merge Sort

Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
Big-O gösterimini yazınız.

### Solution:

Dizi ikiye bölünür: 
[16, 21, 11] ve [8, 12, 22].

Her iki alt dizi ayrı ayrı sıralanır.
    -Sol alt dizi: [11, 16, 21]
    -Sağ alt dizi: [8, 12, 22]

Şimdi iki sıralı alt dizi birleştirilir:
[8, 11, 12, 16, 21, 22]


Big-O Gösterimi: 
O(n log n) - Merge Sort, ortalama ve en kötü durumda da O(n log n) zaman karmaşıklığına sahiptir. Bu, Merge Sort'un genellikle hızlı ve verimli bir sıralama algoritması olarak kabul edilmesinin nedenidir.

*****************************************************************

# Project 3 - Binary Search Tree Projesi

[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

### Solution;

      7
     / \
    5   8
   /   / \
  1   6   9
   \     /
    3   8
     \
      4
     /
    2

Başlangıçta, kök düğüm (root) olan 7'yi seçiyoruz.

Root: 7
7'in sağından gelen ilk düğüm: 5
5'in sağından gelen ilk düğüm: 8
8'in solundan gelen ilk düğüm: 6
5'in solundan gelen ilk düğüm: 1
1'in sağından gelen ilk düğüm: 3
3'in sağından gelen ilk düğüm: 4
1'in solundan gelen ilk düğüm: 0
0'in sağından gelen ilk düğüm: 2
8'in sağından gelen ilk düğüm: 9