# Traffic
![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Traffic/Traffic.png)
## Soru İçeriği
[traffic.7z](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Traffic/traffic.7z)

## Çözüm
Soruda verilen dosyayı çıkartıyoruz.
```
7z x traffic.7z
```
![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Traffic/Screenshot_1.png)

çıkartılan dosyalarda her log dosyası .gz ile arşivlenmiş. Log dosyalarını da .gz den çıkartıyoruz

```
gunzip *
```

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Traffic/Screenshot_2.png)

Soru bize rita kullanmamızı önermiş. Bende rita'yı kurup çalıştırıyorum.

```
rita import 2021-09-08/* huntress_ctf_traffic
```

Oluşturduğumuz raporu incelemek için aşağıdaki kodu yazıyorum.

```
rita html-report huntress_ctf_traffic
```

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Traffic/Screenshot_3.png)

İşaretlenen github sitesini ziyaret ediyorum.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Traffic/Screenshot_4.png)

İşte flag.
