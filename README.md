## Insertion Sort

[22,27,16,2,18,6] dizisinin sort türüne göre aaşamalarını yazalım.

* İlk iki elemana baktığımızda 22>27 olduğundan değişiklik yapmayız.
[22,27,16,2,18,6]

* Üçüncü elemena baktığımızda 27>16 ve 22>16 olduğundan 16 en başa eklenir.
[16,22,27,2,18,6]

* Dördüncü elemanı incelediğimizde 16>2 22>2 27>2 olduğundan 2 dizinin en başına eklenir.
[2,16,22,27,18,16]

* Beşinci elemanımız 18'e baktığımızda 22>18 27>18 olduğundan bu sayıların soluna eklenir.
[2,16,18,22,27,6]

* Son elemanımız olan 6'yı incelersek 16,18,22 ve 27 sayılarından küçük olduğundan bu sayıların soluna aktarılır.
[2,6,16,18,22,27] 

---

## Big-O Gösterimi

İlk adımda (n) eleman, ikinci adımda (n-1) eleman, üçüncü adımda (n-2) eleman ile işlem yaparak 1 eleman kalana kadar devam edilir.

n+(n-1)+(n-2)+...+1= n(n+1) /2

n^2+n /2 elde edilir. n^2 yi alıyoruz. O halde O(n^2) şeklinde gösterilir.

---

## Time Complexity

Time Complexity: Dizi sıralandıktan sonra 18 sayısı average, worst, best case'lerden hangisinin kapsamına girer?

[2,6,16,18,22,27] diziminde 18 sayısı ortada olduğundan average case kapsamına girer.

---

## Selection Sort

[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazalım.

* En küçük sayı en başta olacak şekilde 2 ve 7'nin yerleri değişirilir. [2,3,5,8,7,9,4,15,6]

* 2'den sonra 3 doğru bir sıralamadır. [2,3,5,8,7,9,4,15,6]

* 4 ve 5 yer değiştirir. [2,3,4,8,7,9,5,15,6]

* 5 ve 8 yer değiştirir. [2,3,4,5,7,9,8,15,6]

* 6 ve 7 yer değiştirir. [2,3,4,5,6,9,8,15,7]

* 7 ve 9 yer değiştirir. [2,3,4,5,6,7,8,15,9]

* 8 7'den sonra gelmeli, değişiklik yapılmaz. [2,3,4,5,6,7,8,15,9]

* 9 ve 15 yer değiştirir. [2,3,4,5,6,7,8,9,15]
