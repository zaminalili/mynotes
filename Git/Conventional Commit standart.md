Git commit mesajları **açıq, qısa və anlaşılan** olmalıdır.

## **1. Commit Mesajı Formatı**

```
<type>(<scope>): <subject>

<body> (Məcburi deyil)
<footer> (Məcburi deyil)
```

###  **1.1. `type` (Növ)**

Commit mesajı aşağıdakı növlərdən biri olmalıdır:

- **feat** – Yeni bir xüsusiyyət (feature) əlavə edildikdə
- **fix** – Xəta (bug) düzəldildikdə
- **refactor** – Kodun funksionallığını dəyişmədən refaktor edildikdə
- **perf** – Performans yaxşılaşdırıldıqda
- **test** – Testlər əlavə edildikdə və ya yeniləndikdə
- **docs** – Yalnız sənədləşdirmə (README) dəyişdirildikdə
- **chore** – Təmizlik, dependency yeniləmələri, linting və s.
- **style** – Kod formatlama (məsələn, boşluq, nöqtə-vergül düzəlişləri)

### **1.2. `scope` (Məcburi deyil)**

Dəyişiklik hansı modul və ya hissə ilə bağlıdır?  
Məsələn, **auth**, **api**, **database** kimi modullar göstərilə bilər.

### **1.3. `subject`**

- Cümlə böyük hərflə başlamamalıdır.
- Sonda nöqtə (.) olmamalıdır.
- İndiki zaman feilləri əmr şəklində istifadə edilməlidir (məsələn, _add_, _fix_, _update_).

✅ **Düzgün nümunə:**

```
feat(auth): add JWT authentication
```

❌ **Yanlış nümunə:**

```
Added JWT authentication.
```

### **1.4. `body` (Məcburi deyil)**

Dəyişiklik haqqında əlavə məlumat verilir. Bura **"Niyə?" və "Necə?"** suallarına cavab daxil edilə bilər.

 **Nümunə:**

```
feat(auth): add JWT authentication

Implemented JWT-based authentication using Microsoft Identity.
Now users can log in and get an access token.
```

### **1.5. `footer` (Məcburi deyil)**

Burada **issue tracking, breaking change və digər qeydlər** göstərilir.

**Issue ilə əlaqəli commit:**

```
fix(api): resolve user authentication issue

Fixed a bug causing authentication failures due to missing claims.
Closes #42
```

 **Breaking change (geriyə uyğun olmayan dəyişiklik):**

```
refactor(db): update user table schema

BREAKING CHANGE: Changed column name `username` to `user_name`.
```

---

## **2. Ən Yaxşı Təcrübələr**

1.  50 hərfdən çox olmayan commit başlığı (subject) yaz. 
2.  Başlıqdan sonra boş sətir qoy, sonra bədən hissəsini əlavə et. 
3.  Əmr feillərindən istifadə et (add, fix, update).
4.  Bir commit bir məqsəd daşımalıdır.  
5.  İngilis dilində yazmağa çalış, çünki beynəlxalq komandalar bunu anlayacaq. 
6.  `git commit --amend` ilə səhvləri düzəlt.  
7.  Əhəmiyyətli dəyişikliklər üçün “BREAKING CHANGE” qeyd et.

---

## **3. Real Layihədən Nümunələr**

### **Yeni xüsusiyyət (feat)**

```
feat(profile): allow users to upload avatars
```

 **"Profilə şəkil yükləmə funksiyası əlavə olundu."**

### **Xəta düzəlişi (fix)**

```
fix(auth): resolve token expiration issue
```

**"Tokenin vaxtı bitdikdə yaranan səhv düzəldildi."**

### **Refaktor (refactor)**

```
refactor(user): simplify email validation logic
```

**"Email təsdiqləmə məntiqi sadələşdirildi."**

### **Sənədləşdirmə (docs)**

```
docs(readme): update installation guide
```

**"README faylında quraşdırma təlimatı yeniləndi."**

---

##  **4. Commit Mesajlarını Standartlaşdırmaq üçün Alətlər**

🔹 **Commitlint** – Commit mesajlarının formatını yoxlayır.  
🔹 **Husky** – Commitdən əvvəl avtomatik yoxlama aparır.  
🔹 **Lint-staged** – Yalnız dəyişən faylları lint edir.

