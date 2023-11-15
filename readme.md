# Proyekt Adı: Event Management API

## Proyekt haqqında:

Bu proyektlə, şirkətlərə öz eventləri(tədbirlərini) idarə edə biləcək, eləcə də iştirakçılar həmin bu tədbirlərə qeydiyyatdan keçə biləcək və hətta digər iştirakçılar haqqında məlumat ala biləcək.

## Əsas özəllikləri:

1. **Login/Register:**

   - JWT tokenlər istifadə edilərək sistemə giriş və çıxışın idarə edilməsi
   - Həm şirkətlər(təşkilatçılar) üçün həm də iştirakçılar üçün ayrı login və register

2. **Tədbirlər:**
   - Tədbirlərin CRUD-ı
   - Tədbirlərdə olmalı olan xüsusiyyətlər: başlıq, açıqlama, keçirləcəyi tarix və vaxt, məkan və tədbirə aid şəkillər
   - Tədbirlərin özləri müəyyən kateqoriyaya aid olmalıdır məsələn teambuilding, bayram və sair
3. **İştirakçılar üçün qeydiyyat və biletlər:**
   - İştirakçılar rahatlıqla istədikləri tədbirə qeydiyyatdan keçə bilərlər(əgər yer qalıbsa)
   - Ödəmədən sonra onlara üç cür bilet göndərilməlidir:
     - E-mail vasitəsilə(əgər mail serveri yoxdursa olmasa
       olar)
       > E-mail dəvətnaməsi yazı və pdf şəklində olmalıdır
     - Qr code spesifik bilet üçün
     - HTML formatında hazırlanmış bilet(veb client-lar üçün)
4. **Tədbir sonrası iştirakçı rəyləri:**
   - Sadəcə tədbirdə iştirak etmiş iştirakçılar, tədbir haqqında rəylər yaza bilər və onu dəyərləndirə bilərlər(ulduz ilə)
   - Hələ baş verməmiş tədbirin iştirakçıları isə onu paylaşa biləcəklər(xüsusi bir link ilə)
5. **Tədbir analitikası:**
   - Tədbirdə iştirak edənlərə görə müxtəlif statistikalar çıxarın. Məsələn iştirak edən kişilərin sayı kimi
6. **Tədbirlərin əlçatımlılığı:**
   - Bəzi tədbirlər, hər kəsə açıq ola bilir lakin bəzi tədbirlər xüsusi linklə olmalıdır bu məqsədlə təşkilatçılar üçün bir endpoint olmalıdır
