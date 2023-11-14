# Wimble(Forensic)
![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Wimble/Wimble_soru.png)
## Soru İçeriği
[wimble.7z](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Wimble/wimble.7z)

## Çözüm
Bir arşiv dosyasının içerisinde "fetch" isimli bir vim dosyası verilmiş. Vim uzantılı dosyaları 7zip uygulaması ile çıkartabiliyoruz. Dosyayı çıkarttıktan  sonra klasörün içerisinde tekrardan "fetch" isimli bir arşiv klasörü bulunuyor. Onu da arşivden çıkartıyoruz.

![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Wimble/wimble2.PNG)

Windows log dosyaları verilmiş. Bunları kolaylıkla inceleyebileceğimiz Zinnermach 'ın PECmd prefetch parser toolunu kullanıyoruz. Toolu çalıştırıp stringleri arattığımızda flagı buluyoruz. 
``` PECmd.exe -d fetch\ | select-string "flag" ```

![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Wimble/Wimble.png)

```FLAG{97F33C9783C21DF85D79D613B0B258BD}```
