# Indirect Payload
![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/F12/Screenshot_1.png)
## Soru İçeriği
Online Soru

## Çözüm
![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Indirect_Payload/Screenshot_1.png)

Sitedeki butona basıldığı zaman bir sürü istek dönüyor ama çok hızlı olduğu için hiçbirini göz ile yakalayamıyorum. Bu yüzden burp ile araya girip giden gelen istekleri inceliyorum.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Indirect_Payload/Screenshot_2.png)

İsteklere baktığımız zaman birbirinden farklı pathlere sırayla yönlendirme yaptığını görüyoruz. Bu pathlerin içeriğine baktığımız zaman "character 0 of the payload is f" yazsını görüyoruz.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Indirect_Payload/Screenshot_3.png)

Yani bir dizi karakterlerin yerlerini gösteriyor. Sırayla isteklere baktığımız zaman ve harfleri birleştirdiğimiz zaman flag ortaya çıkıyor.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Indirect_Payload/Screenshot_4.png)
