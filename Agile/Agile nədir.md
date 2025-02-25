Çevik metodologiya, işi kiçik, idarə oluna bilən hissələrə ayıran, davamlı əməkdaşlığı, təkmilləşdirməni və müştəri məmnuniyyətini vurğulayan layihə idarəetmə yanaşmasıdır. 

**Ənənəvi (waterflow) yanaşma**
Təsəvvür edək ki, bir ev tikmək istəyirik:

Bu yanaşma ilə ev tikmək, əvvəlcə hər şeyi detallı şəkildə planlaşdırmaq və sonra ardıcıl addımlarla həyata keçirmək kimidir:
1. **Planlama:** Bir memar hər detalı planlaşdırır, bütün ölçüləri müəyyən edir, materialları seçir.
2. **Dizayn:** Ev üçün detallı rəsmlər, elektrik və su xətləri, otaqların ölçüləri əvvəlcədən təyin edilir.
3. **İcra:** Tikinti başlayır və plan üzrə mərhələli şəkildə irəliləyir. Əvvəlcə fundament, sonra divarlar, dam və s.
4. **Təslim:** İş tam bitəndən sonra müştəriyə təhvil verilir.

Əgər bu prosesin ortasında kimsə desə ki, “Mənim üçün bir əlavə otaq tikin” və ya “Mətbəxin yerini dəyişək”, bu çox çətin və bahalı ola bilər, çünki bütün sistem əvvəlcədən planlaşdırılıb.

![[Pasted image 20250220141858.png]]

**Agile yanaşması**
Agile yanaşması ilə ev tikmək, əvvəlcə əsas strukturu qurmaq və sonra ehtiyaca uyğun olaraq mərhələ-mərhələ inkişaf etdirmək kimidir:
1. **Minimal İşlək Ev:** Əvvəlcə sadə, yaşamaq üçün kifayət qədər rahat bir ev tikilir (məsələn, 1 otaq, mətbəx və hamam).
2. **Rəy və Düzəlişlər:** Ev sahibi içəridə yaşamağa başlayır və hansı dəyişikliklərə ehtiyac olduğunu görür.
3. **İnkişaf:** Lazım gəldikcə əlavə otaqlar tikilir, bəzək işləri aparılır, mətbəx böyüdülür və s.
4. **Daimi Adaptasiya:** Əgər müştəri evə yeni smart ev texnologiyaları əlavə etmək istəsə və ya dizaynı dəyişmək istəsə, bu daha asan olur, çünki sistem modular şəkildə qurulub.

Bu yanaşmada müştəri daim prosesdə iştirak edir və hər iterasiyada istifadə oluna bilən bir nəticə əldə edilir. Nəticədə, ehtiyaclar dəyişdikcə layihəyə uyğunlaşmaq mümkün olur.

![[Pasted image 20250220125716.png]]

```flowchart LR
    subgraph "Agile Lifecycle"
        direction TB
        
        Plan["Plan"] -->|"Define Work"| Exec["Execute"]
        Exec -->|"Deliver Value"| Eval["Evaluate"]
        Eval -->|"Gather Feedback"| Plan
        
        style Plan fill:#90EE90,stroke:#006400,color:#000000
        style Exec fill:#ADD8E6,stroke:#00008B,color:#000000
        style Eval fill:#FFB6C1,stroke:#8B0000,color:#000000
    end
```

Çevik həyat dövrünün hər bir mərhələsi müəyyən bir məqsədə xidmət edir:

**Planlaşdırma**: Qarşıdan gələn sprint üçün iş elementlərini müəyyənləşdirir və prioritetləşdirir
**İcra etmək**: Planlaşdırılmış iş elementlərini tamamlayır və dəyərə çatdırır
**Qiymətləndirmək**: İnkişaf nəzərdən keçirilir, rəy toplanılır və təkmilləşdirmələr müəyyənləşdirilir.

## [[Agile əsas dəyərləri və prinsipləri]]


## Common Agile Methodologies

Çevik prinsiplərin ən çox tətbiq olunan üsulları:

 **[[0 Scrum]]**
	 - Sabit uzunluqlu təkrarlanan dövrlərdən (sprintlərdən) istifadə edir 
	 - Scrum Master və Product Owner kimi rolları ehtiva edir
	 - Gündəlik ayaqüstü (stand-up) görüşlərini təqdim edir
 **Kanban**
	 - Lövhə və kartlardan istifadə etməklə vizual yanaşma
	 - Sabit təkrarlar yoxdur
	 - Davamlı iş axınına diqqət yetirir

## Üstünlükləri
Agile yanaşmanın bir necə üstünlükləri var:
- **Elastiklik**: Dəyişən tələblərə tez uyğunlaşır
- **Təkmilləşdirilmiş Əməkdaşlıq:** Komanda ünsiyyətini və əməkdaşlığı gücləndirir
- **Müştəri Fokuslu:** Müştəri ehtiyaclarına uyğun dəyər verir
- **Keyfiyyət Təminatı:** Daimi sınaq və davamlı təkmilləşdirmə
- **Risklərin idarə edilməsi:** problemlərin erkən müəyyən edilməsi və azaldılmağı

## Real dünya tətbiqi
Facebook, Google və Amazon kimi böyük şirkətlər Agile metodologiyasından uğurla istifadə edirlər, çünki:
- Bazar dəyişikliklərinə sürətli reaksiya verir
- Müştərilərə tez-tez rəy (feedback) imkanları təqdim edir
- Davamlı təkmilləşdirməni dəstəkləyir
- Resurslardan səmərəli istifadəni təşviq edir

>Çevik sadəcə bir metodologiya deyil - bu, davamlı təkmilləşdirmə və müştəri məmnuniyyəti vasitəsilə dəyər təqdim etməyə yönəlmiş bir zehniyyətdir (yanaşmadır). Onun iterativ yanaşması yüksək keyfiyyət və səmərəliliyi qoruyarkən layihələrin dəyişən tələblərə uyğun olmasını təmin edir.
# Çevik metodun öyrənmə və tədrisə tətbiqi


İstinadlar
[asana.com](https://asana.com/resources/agile-methodology)
[geeksforgeeks.org](https://www.geeksforgeeks.org/what-is-agile-methodology/)
Analogiya: chatgpt 4o