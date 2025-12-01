# 📚 SmartLibrary — Akıllı Kütüphane Yönetim Sistemi

Java + SQLite ile geliştirilmiş **hafif, hızlı ve sade** bir kütüphane yönetim uygulaması! ☕📘
Kitap, öğrenci ve ödünç işlemlerini tek bir terminal uygulamasında kolayca yönetebilirsin. 🚀

---

## ✨ Özellikler

* 📘 **Kitap Yönetimi:** Ekle, listele, sil
* 👤 **Öğrenci Yönetimi:** Ekle, listele, sil
* 🔄 **Ödünç & İade İşlemleri**
* 🗃 **SQLite Veritabanı Desteği**
* 🧩 **Temiz Model – Repository Yapısı**
* ⚡ **Basit Terminal Arayüzü**

---

## 🛠 Kullanılan Teknolojiler

* ☕ **Java (JDK 8/17)**
* 🗃 **SQLite Database**
* 🔌 **SQLite JDBC Driver**
* 🏗 **Nesne Yönelimli Programlama (OOP)**

---

## 📁 Proje Yapısı

```
SmartLibrary/
 ├─ smartlibrary.db
 ├─ sqlite-jdbc-3.xx.jar
 ├─ Main.java
 ├─ Database.java
 ├─ Models/ (Book, Student, Loan)
 └─ Repositories/ (BookRepository, StudentRepository, LoanRepository)
```


---

## 🧭 Menü Yapısı

* ➕ Kitap Ekle
* 📚 Kitapları Listele
* ➕ Öğrenci Ekle
* 🧑‍🎓 Öğrencileri Listele
* 🔄 Kitap Ödünç Ver
* 📋 Ödünç Listesi
* ↩️ Kitap Geri Al
* ❌ Kitap Sil
* ❌ Öğrenci Sil

---

## 🗄️ Veritabanı Tabloları


### 📘 **Books**

| id (PK) | title     | author | year       |
| ------- | --------- | ------ | ---------- |
| Auto    | Kitap Adı | Yazar  | Basım Yılı |

### 👤 **Students**

| id (PK) | name        | department |
| ------- | ----------- | ---------- |
| Auto    | Öğrenci Adı | Bölüm      |

### 🔄 **Loans**

| id (PK) | bookId (FK) | studentId (FK) | dateBorrowed | dateReturned                |
| ------- | ----------- | -------------- | ------------ | --------------------------- |
| Auto    | Kitap ID    | Öğrenci ID     | Alınan Tarih | İade Tarihi (Null olabilir) |

---
## 📥 Kurulum

1. **Projeyi indir / klonla**:

```bash
git clone https://github.com/TimaYT/SmartLibrary.git
```

2. **JDBC driver'ı ekle** (lib klasöründen)
3. `Main.java` → ▶️ Çalıştır


---


## 🚀 Çalıştırma

### 1) JDBC Bağımlılığını Ekle

VS Code → **JAVA PROJECTS** → *Referenced Libraries* → **+** → `.jar` dosyasını seç.

### 2) Uygulamayı Başlat

`Main.java` → ▶️ **Run** (veya `F5`)
Terminalde menü otomatik olarak görünür. ✔️


---

## 👤 Geliştirici

**Yasin Balkan**
🌐 GitHub: [https://github.com/TimaYT](https://github.com/TimaYT)

