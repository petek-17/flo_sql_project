# flo_sql_project
# 🧠 SQL ile FLO Müşteri Analizi

Bu proje, FLO perakende verisi üzerinden SQL sorguları ile müşteri davranışlarının ve satış performansının analizini kapsamaktadır. Analizler, `Customers` isimli bir veritabanında oluşturulan `FLO` adlı tablo üzerinden gerçekleştirilmiştir.

## 🧾 Proje Amacı

- FLO müşterilerinin alışveriş davranışlarını analiz etmek
- Ciro, alışveriş kanalı, müşteri kategorileri gibi çeşitli metrikleri SQL sorguları ile incelemek
- İş zekası raporlamaları için veri hazırlığına katkıda bulunmak

---

## 🧱 FLO Tablosunun Yapısı

```sql
CREATE DATABASE Customers;

USE Customers;

CREATE TABLE FLO (
    master_id VARCHAR(50),
    order_channel VARCHAR(20),
    last_order_channel VARCHAR(20),
    first_order_date DATE,
    last_order_date DATE,
    order_num_total_ever_online INT,
    order_num_total_ever_offline INT,
    customer_value_total_ever_online FLOAT,
    customer_value_total_ever_offline FLOAT,
    interested_in_categories_12 TEXT,
    store_type VARCHAR(30)
);


 1. Customers isimli bir veritabanı ve verilen veri setindeki değişkenleri içerecek FLO isimli bir tablo oluşturunuz.
 2. Kaç farklı müşterinin alışveriş yaptığını gösterecek sorguyu yazınız. 
3. Toplam yapılan alışveriş sayısı ve ciroyu getirecek sorguyu yazınız.
 4. Alışveriş başına ortalama ciroyu getirecek sorguyu yazınız. 
5. En son alışveriş yapılan kanal (last_order_channel) üzerinden yapılan alışverişlerin toplam ciro ve alışveriş sayılarını 
getirecek sorguyu yazınız.  
6. Store type kırılımında elde edilen toplam ciroyu getiren sorguyu yazınız. 
7. Yıl kırılımında alışveriş sayılarını getirecek sorguyu yazınız (Yıl olarak müşterinin ilk alışveriş tarihi (first_order_date) yılını 
baz alınız)
 8. En son alışveriş yapılan kanal kırılımında alışveriş başına ortalama ciroyu hesaplayacak sorguyu yazınız.  
SORULAR
 MIUULTM
 www.miuul.com
 Copyright © Miuul, Inc. All Rights Reserved
 9. Son 12 ayda en çok ilgi gören kategoriyi getiren sorguyu yazınız.
 10. En çok tercih edilen store_type bilgisini getiren sorguyu yazınız.  
11. En son alışveriş yapılan kanal (last_order_channel) bazında, en çok ilgi gören kategoriyi ve bu kategoriden ne kadarlık 
alışveriş yapıldığını getiren sorguyu yazınız.
 12. En çok alışveriş yapan kişinin ID’ sini getiren sorguyu yazınız. 
13. En çok alışveriş yapan kişinin alışveriş başına ortalama cirosunu ve alışveriş yapma gün ortalamasını (alışveriş sıklığını) 
getiren sorguyu yazınız. 
14. En çok alışveriş yapan (ciro bazında) ilk 100 kişinin alışveriş yapma gün ortalamasını (alışveriş sıklığını) getiren sorguyu 
yazınız. 
15. En son alışveriş yapılan kanal (last_order_channel) kırılımında en çok alışveriş yapan müşteriyi getiren sorguyu yazınız. 
16. En son alışveriş yapan kişinin ID’ sini getiren sorguyu yazınız. (Max son tarihte birden fazla alışveriş yapan ID bulunmakta. 
Bunları da getiriniz.) 
