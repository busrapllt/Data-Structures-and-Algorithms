Proje 1
[22,27,16,2,18,6] -> Insertion Sort
Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
Big-O gösterimini yazınız.
Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız
1.	Average case: Aradığımız sayının ortada olması
2.	Worst case: Aradığımız sayının sonda olması
3.	Best case: Aradığımız sayının dizinin en başında olması
[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

CEVAPLAR:

Insertion Sort’un mantığı, diziyi adım adım sıralar. İşte verilen [22, 27, 16, 2, 18, 6] dizisinin Insertion Sort algoritmasına göre sıralama aşamaları aşağıdaki gibidir:

İlk eleman (22) zaten sıralı kabul edilir.

Step 1: [22, 27, 16, 2, 18, 6]
İkinci eleman (27), ilk elemanla karşılaştırılır ve yerinde kalır.

Step 2: [22, 27, 16, 2, 18, 6]
Üçüncü eleman (16), sıralı alt diziye (22, 27) eklenir:

16, 27'den küçüktür, bu yüzden 27'nin önüne yerleştirilir.
16, 22'den de küçüktür, bu yüzden 22'nin önüne yerleştirilir.

Step 3: [16, 22, 27, 2, 18, 6]
Dördüncü eleman (2), sıralı alt diziye (16, 22, 27) eklenir:

2, 27'den küçüktür, bu yüzden 27'nin önüne yerleştirilir.
2, 22'den de küçüktür, bu yüzden 22'nin önüne yerleştirilir.
2, 16'dan da küçüktür, bu yüzden 16'nın önüne yerleştirilir.

Step 4: [2, 16, 22, 27, 18, 6]
Beşinci eleman (18), sıralı alt diziye (2, 16, 22, 27) eklenir:

18, 27'den küçüktür, bu yüzden 27'nin önüne yerleştirilir.
18, 22'den de küçüktür, bu yüzden 22'nin önüne yerleştirilir.
18, 16'dan büyüktür, bu yüzden yerinde kalır.
	

Step 5: [2, 16, 18, 22, 27, 6]
Altıncı eleman (6), sıralı alt diziye (2, 16, 18, 22, 27) eklenir:

6, 27'den küçüktür, bu yüzden 27'nin önüne yerleştirilir.
6, 22'den de küçüktür, bu yüzden 22'nin önüne yerleştirilir.
6, 18'den de küçüktür, bu yüzden 18'in önüne yerleştirilir.
6, 16'dan da küçüktür, bu yüzden 16'nın önüne yerleştirilir.
6, 2'den büyüktür, bu yüzden yerinde kalır.

En Son Elde Edilen Dizi: [2, 6, 16, 18, 22, 27]


Big-O Gösterimi:

Insertion Sort'un en kötü durumdaki zaman karmaşıklığı O(n²)'dir. Bunun nedeni, her eklemede en kötü durumda dizinin geri kalanını kaydırmak zorunda kalmamızdır.

18 Sayısının Time Complexity Durumu:

Sıralanmış dizide [2, 6, 16, 18, 22, 27] şeklinde, 18 sayısının konumu ortada olduğundan, average case (ortalama durum) kapsamına girer


Selection Sort Adımları:

Verilen dizi: [7, 3, 5, 8, 2, 9, 4, 15, 6]

Selection Sort, her adımda en küçük elemanı bulup başa koyarak ilerler. İlk dört adımı aşağıdaki gibidir:

İlk adımda en küçük eleman (2) bulunur ve ilk sıraya yerleştirilir.

Dizi: [2, 3, 5, 8, 7, 9, 4, 15, 6]
İkinci adımda, geri kalan kısmın en küçük elemanı (3) zaten yerindedir.

Dizi: [2, 3, 5, 8, 7, 9, 4, 15, 6]
Üçüncü adımda, geri kalan kısmın en küçük elemanı (4) bulunur ve üçüncü sıraya yerleştirilir.

Dizi: [2, 3, 4, 8, 7, 9, 5, 15, 6]
Dördüncü adımda, geri kalan kısmın en küçük elemanı (5) bulunur ve dördüncü sıraya yerleştirilir.

Dizi: [2, 3, 4, 5, 7, 9, 8, 15, 6]
Bu adımlarla Selection Sort algoritmasının ilk dört adımı tamamlanmış olur.


