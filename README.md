# Insertion Sort Ödevi

[22,27,16,2,18,6] -> Insertion Sort

### Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

-Step-1: [22,*27*,16,2,18,6] => 22 elemanı bir sıralama işlemine tabi tutulmaz. Sıralama işlemi, ikinci eleman olan 27 ile başlar. 27, 22'den büyük olduğu için yer değiştirmez.

-Step-2: [22,27,*16*,2,18,6] => 16 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [16,22,27,2,18,6]

-Step-3: [16,22,27,*2*,18,6] => 2 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [2,16,22,27,18,6]

-Step-4: [2,16,22,27,*18*,6] => 18 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [2,16,18,22,27,6]

-Step-5: [2,16,18,22,27,*6*] => 6 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [2,6,16,18,22,27]

***************************************************************

### Big-O gösterimini yazınız.
   
-Step-1'de, bütün elemanları gözden geçirip en küçüğünü buluyoruz. Bu yüzden Step-1'de yapılan işlem sayısı = n.

-Step-2'de, 2 hariç tüm elemanları gözden geçirip en küçüğünü buluyoruz. Bu yüzden Step-2'de yapılan işlem sayısı = n-1.

-Step-3'de, 2 ve 6 hariç tüm elemanları gözden geçirip en küçüğünü buluyoruz. Bu yüzden Step-3'de yapılan işlem sayısı = n-2.

-Bu şekilde devam ettiği zaman toplamda yapılan işlem sayısı = O(n^2)

***************************************************************

### Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız.

-Average case: Aradığımız sayının ortada olması
  
-Worst case: Aradığımız sayının sonda olması
  
-Best case: Aradığımız sayının dizinin en başında olması.

=> Aradığımız sayı ortalarda olduğu için Average Case.

***************************************************************

### [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.
   
-Step-1: [7,*3*,5,8,2,9,4,15,6] => 3 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [3,7,5,8,2,9,4,15,6]

-Step-2: [3,7,*5*,8,2,9,4,15,6] => 5 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [3,5,7,8,2,9,4,15,6]

-Step-3: [3,5,7,*8*,2,9,4,15,6] => 8 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [3,5,7,8,2,9,4,15,6]

-Step-4: [3,5,7,8,*2*,9,4,15,6] => 2 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [3,5,7,2,8,9,4,15,6]

***************************************************************

# Merge Sort Ödevi
[16,21,11,8,12,22] -> Merge Sort

### Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
[16,21,11,8,12,22]

[16,21,11]   |   [8,12,22]

[16,21]   |   [11]   |   [8,12]   |   [22]

[16]      [21]   |   [11]   |   [8]      [12]   |   [22]

[16,21]   |   [11]   |   [8,12]   |   [22]

[11,16,21]   |   [8,12,22]

[8,11,12,16,21,22]

***************************************************************

### Big-O gösterimini yazınız.
Diziyi parçalara bölmek, logn işlem gerektirir. Parçaları birleştirme esnasında bütün elemanların karşılaştırılması ise n işlem gerektirir. Bu yüzden Merge Sort algoritmasının Big-O gösterimi = O(nlogn)

***************************************************************

# Binary Search Tree Ödevi
[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

        7
       / \
      5   8
     / \    \
    1   6    9
   / \
  0   3
     / \
    2   4
