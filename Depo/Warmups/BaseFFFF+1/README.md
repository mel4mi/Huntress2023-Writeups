# BaseFFFF+1
![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/BaseFFFF%2B1/BaseFFFF%2B1.png)
## Soru İçeriği
![Soru_icerigi](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/BaseFFFF%2B1/Screenshot_4.png)


## Çözüm

Soruyu anlamak için önce soru başlığını 3 parçaya ayırmak lazım. Bunlar: "Base" + "FFFF" + "+1" ibareleridir. Base ibaresi güncel olarak çokça kullanılan veri taşıma veya saklamak için kullanılan bir kodlama sistemine aittir. FFFF ibaresi ise Hexadecimal bir sayı ibaresidir. Çözüm için FFFF değerini decimale çevirip en sondaki +1'i eklememiz gerekiyor.

![FFFF_Deger](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/BaseFFFF%2B1/Screenshot_1.png)




65535 + 1 = 65536, çıkan sonucu base65536 olarak aratalım.

![Google](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/BaseFFFF%2B1/Screenshot_2.png)

Encode edilmiş metni çevirelim.

![Flag](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/BaseFFFF%2B1/Screenshot_3.png)


İşte flag.
