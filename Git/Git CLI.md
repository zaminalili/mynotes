Git CLI (Command Line Interface) ilə əsas git əmrləri və istifadəsi aşağıdakı kimi həyata keçirilir:
### 1. **Git Konfiqurasiyası (Config)**

İlk dəfə Git quraşdırdıqda istifadəçi adı və email təyin etmək lazımdır:

```sh
git config --global user.name "Adınız"
git config --global user.email "email@example.com"
```

Konfiqurasiyanı yoxlamaq üçün:

```sh
git config --list
```

---

### 2. **Git Deposu (Repository) Yaratmaq və ya Klonlamaq**

#### Yeni git layihəsi yaratmaq:

```sh
git init
```

Bu əmrlə cari qovluqda `.git` adlı gizli qovluq yaradılır və bu, Git deposu olur.

#### Mövcud depodan klonlamaq:

```sh
git clone https://github.com/user/repository.git
```

---

### 3. **Dəyişiklikləri İzləmək və Yoxlamaq**

#### Hansı faylların dəyişdiyini görmək:

```sh
git status
```

#### Dəyişiklikləri göstərmək:

```sh
git diff
```

---

### 4. **Faylları İzlənməyə (Staging) Əlavə Etmək**

#### Tək faylı əlavə etmək:

```sh
git add fayl_adi
```

#### Bütün faylları əlavə etmək:

```sh
git add .
```

---

### 5. **Dəyişiklikləri Yadda Saxlamaq (Commit)**

#### Dəyişiklikləri commit etmək:

```sh
git commit -m "Mövzunu qısaca izah edən mesaj"
```

#### Əvvəlki commit mesajını dəyişmək:

```sh
git commit --amend -m "Yeni mesaj"
```

---

### 6. **Dəyişiklikləri Uzaq (Remote) Depoya Göndərmək**

#### Uzaq depoya bağlantı əlavə etmək:

```sh
git remote add origin https://github.com/user/repository.git
```

#### Dəyişiklikləri uzaq depoya göndərmək:

```sh
git push origin main
```

(`main` və ya `master` şaxəsini göndərmək üçün)

---

### 7. **Uzaq Depodan Dəyişiklikləri Çəkmək**

#### Ən son dəyişiklikləri gətirmək:

```sh
git pull origin main
```

#### Uzaq depodan dəyişiklikləri yükləmək, amma merge etməmək:

```sh
git fetch origin
```

---

### 8. **Şaxələrlə (Branch) İşləmək**

#### Yeni şaxə yaratmaq:

```sh
git branch yeni-saxe
```

#### Şaxəni dəyişmək:

```sh
git checkout yeni-saxe
```

və ya yeni metod:

```sh
git switch yeni-saxe
```

#### Şaxə yaratmaq və keçid etmək:

```sh
git checkout -b yeni-saxe
```

və ya

```sh
git switch -c yeni-saxe
```

#### Şaxəni uzaq depoya göndərmək:

```sh
git push -u origin yeni-saxe
```

#### Şaxələri siyahıya almaq:

```sh
git branch
```

#### Uzaq şaxələri göstərmək:

```sh
git branch -r
```

#### Şaxəni silmək:

```sh
git branch -d yeni-saxe
```

#### Uzaq şaxəni silmək:

```sh
git push origin --delete yeni-saxe
```

---

### 9. **Merge və Rebase**

#### Başqa şaxəni `main` şaxəsinə merge etmək:

```sh
git checkout main
git merge yeni-saxe
```

#### `rebase` ilə şaxəni yeniləmək:

```sh
git checkout yeni-saxe
git rebase main
```

---

### 10. **Commitləri Geri Çəkmək və Ləğv Etmək**

#### Sonuncu commiti ləğv etmək, amma dəyişiklikləri saxlamaq:

```sh
git reset --soft HEAD~1
```

#### Sonuncu commiti tamamilə ləğv etmək:

```sh
git reset --hard HEAD~1
```

#### Dəyişiklikləri geri qaytarmaq (unstage etmək):

```sh
git restore --staged fayl_adi
```

#### Commit olunmuş bir dəyişiklikdən geri dönmək:

```sh
git revert commit_id
```

---

### 11. **Git Stash (Müvəqqəti Saxlama)**

#### Dəyişiklikləri müvəqqəti saxlamaq:

```sh
git stash
```

#### Sonuncu stash-ı geri gətirmək:

```sh
git stash pop
```

#### Stash siyahısını görmək:

```sh
git stash list
```

#### Müəyyən stash-ı geri gətirmək:

```sh
git stash apply stash@{0}
```

---

### 12. **Git Log və Tarixçəyə Baxmaq**

#### Commit tarixçəsini göstərmək:

```sh
git log
```

#### Qısaldılmış commit siyahısı:

```sh
git log --oneline --graph --all
```

---

### 13. **Git Tag (Etiketləmə)**

#### Yeni tag yaratmaq:

```sh
git tag v1.0.0
```

#### Tag siyahısına baxmaq:

```sh
git tag
```

#### Tag-i uzaq depoya göndərmək:

```sh
git push origin v1.0.0
```

#### Tag-i silmək:

```sh
git tag -d v1.0.0
git push origin --delete v1.0.0
```

---

### 14. **Submodule ilə İşləmək**

#### Layihəyə submodule əlavə etmək:

```sh
git submodule add https://github.com/user/submodule-repo.git path/to/submodule
```

#### Submodule-ləri yeniləmək:

```sh
git submodule update --init --recursive
```

---

### 15. **Git Ignore və Untracked Fayllar**

`.gitignore` faylı yaradıb lazımsız faylları Git-dən kənarda saxlamaq mümkündür:

```sh
echo "node_modules/" >> .gitignore
```

Git ignore fayllarını yoxlamaq:

```sh
git check-ignore -v fayl_adi
```

