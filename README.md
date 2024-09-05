# patika-dev-veri-yap-alg

[22,27,16,2,18,6] -> Insertion Sort

1) Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

-Step-1: [22,*27*,16,2,18,6] => 22 elemanı bir sıralama işlemine tabi tutulmaz. Sıralama işlemi, ikinci eleman olan 27 ile başlar. 27, 22'den büyük olduğu için yer değiştirmez.

-Step-2: [22,27,*16*,2,18,6] => 16 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [16,22,27,2,18,6]

-Step-3: [16,22,27,*2*,18,6] => 2 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [2,16,22,27,18,6]

-Step-4: [2,16,22,27,*18*,6] => 18 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [2,16,18,22,27,6]

-Step-5: [2,16,18,22,27,*6*] => 6 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [2,6,16,18,22,27]

***************************************************************

2) Big-O gösterimini yazınız.
   
-Step-1'de, bütün elemanları gözden geçirip en küçüğünü buluyoruz. Bu yüzden Step-1'de yapılan işlem sayısı = n.

-Step-2'de, 2 hariç tüm elemanları gözden geçirip en küçüğünü buluyoruz. Bu yüzden Step-2'de yapılan işlem sayısı = n-1.

-Step-3'de, 2 ve 6 hariç tüm elemanları gözden geçirip en küçüğünü buluyoruz. Bu yüzden Step-3'de yapılan işlem sayısı = n-2.

-Bu şekilde devam ettiği zaman toplamda yapılan işlem sayısı = O(n^2)

***************************************************************

3) Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız.

-Average case: Aradığımız sayının ortada olması
  
-Worst case: Aradığımız sayının sonda olması
  
-Best case: Aradığımız sayının dizinin en başında olması.

=> Aradığımız sayı ortalarda olduğu için Average Case.

***************************************************************

4) [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.
   
-Step-1: [7,*3*,5,8,2,9,4,15,6] => 3 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [3,7,5,8,2,9,4,15,6]

-Step-2: [3,7,*5*,8,2,9,4,15,6] => 5 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [3,5,7,8,2,9,4,15,6]

-Step-3: [3,5,7,*8*,2,9,4,15,6] => 8 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [3,5,7,8,2,9,4,15,6]

-Step-4: [3,5,7,8,*2*,9,4,15,6] => 2 elemanı seçilir. Kendisinden küçük bir elemana denk gelinceye kadar sola kaydırılır. => [3,5,7,2,8,9,4,15,6]
