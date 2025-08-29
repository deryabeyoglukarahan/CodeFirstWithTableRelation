# 📝 Code First Relation

Bu proje, **Entity Framework Core** kullanılarak **Code First yaklaşımı** ile **ilişkili tablolar** oluşturmayı amaçlamaktadır.  
Proje kapsamında **User** ve **Post** tabloları arasında **bire-çok (One-to-Many)** ilişki kurulmuştur.

---

## 📂 Proje Gereksinimleri

- **ORM Aracı**: Entity Framework Core  
- **Yaklaşım**: Code First  
- **Context Sınıfı**: `PatikaSecondDbContext`  
- **Veri Tabanı İsmi**: `PatikaCodeFirstDb2`  
- **Tablolar**: `Users`, `Posts`  
- **İlişki**:  
  - Bir **User** birden fazla **Post** yazabilir.  
  - Her **Post** yalnızca bir **User**’a aittir.  

---

## 👤 User Tablosu

| Kolon    | Tip    | Açıklama                         |
|----------|--------|----------------------------------|
| Id       | int    | Birincil anahtar, otomatik artan |
| Username | string | Kullanıcının kullanıcı adı       |
| Email    | string | Kullanıcının e-posta adresi      |

---

## 📝 Post Tablosu

| Kolon   | Tip    | Açıklama                              |
|---------|--------|---------------------------------------|
| Id      | int    | Birincil anahtar, otomatik artan      |
| Title   | string | Gönderinin başlığı                    |
| Content | string | Gönderinin içeriği                    |
| UserId  | int    | Gönderinin ait olduğu kullanıcının Id’si |

---
