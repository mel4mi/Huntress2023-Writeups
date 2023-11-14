# Wimble(Forensic)
#### Zorluk: Easy

## Soru
![Soru](https://github.com/K4lender/HuntressCTF23_WriteUps/blob/main/Forensics/Wimble/Wimble.png)

## Çözüm
Bir arşiv dosyasının içerisinde "fetch" isimli bir vim dosyası verilmiş. Vim uzantılı dosyaları 7zip uygulaması ile çıkartabiliyoruz. Dosyayı çıkarttıktan  sonra klasörün içerisinde tekrardan "fetch" isimli bir arşiv klasörü bulunuyor. Onu da arşivden çıkartıyoruz.

![Soru](https://github.com/K4lender/HuntressCTF23_WriteUps/blob/main/Forensics/Wimble/wimble2.PNG)

Windows log dosyaları verilmiş. Bunları kolaylıkla inceleyebileceğimiz Zinnermach 'ın PECmd prefetch parser toolunu kullanıyoruz. Toolu çalıştırıp stringleri arattığımızda flagı buluyoruz. 
``` PECmd.exe -d fetch\ | select-string "flag" ```

![Soru](https://github.com/K4lender/HuntressCTF23_WriteUps/blob/main/Forensics/Wimble/wimble.PNG)

```FLAG{97F33C9783C21DF85D79D613B0B258BD}```
