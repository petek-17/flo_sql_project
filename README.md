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



