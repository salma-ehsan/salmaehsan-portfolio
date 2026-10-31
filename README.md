# Salma Ehsan — Portfolio

موقع بورتفوليو شخصي لـ **Salma Ehsan** — Graphic Designer & Brand Identity Specialist.

موقع صفحة واحدة (Single Page) مبني بـ HTML + CSS + JavaScript فقط، بدون أي أدوات بناء، وجاهز للرفع على GitHub Pages.

---

## شكل المجلد

```
Salma-Portfolio/
├── index.html                 ← الموقع كامل (HTML + CSS + JS)
├── README.md
└── assets/
    ├── images/
    │   ├── profile.jpg        ← صورتك في أول الصفحة (Hero)
    │   ├── about.jpg          ← صورتك في قسم About Me
    │   ├── instructor.jpg     ← بوستر C++ Instructor
    │   ├── logo.png           ← لوجو Rattebhali (براندنج)
    │   ├── burger1.jpg        ← NEW BURGER
    │   ├── burger2.jpg        ← HOT & FRESH BURGER
    │   ├── python1.jpg        ← Python Level 1
    │   ├── python2.jpg        ← Python for High School
    │   ├── python3.jpg        ← Python Level 1 – Neon
    │   ├── scratch.jpg        ← Scratch Course for Kids
    │   ├── comingsoon.jpg     ← Coming Soon – Rattebhali
    │   ├── cpp1.jpg           ← Learn to Code C++
    │   └── cpp2.jpg           ← C++ Course – Chess
    └── files/
        └── Salma_Ehsan_CV.pdf ← السيرة الذاتية
```

> كل الصور والأعمال والـ CV موجودة بالفعل داخل المجلد وجاهزة.

---

## إزاي تعدّلي المحتوى؟

كل النصوص القابلة للتعديل موجودة في **آخر `index.html`** داخل الكائن:

```js
const PORTFOLIO_CONFIG = { ... };
```

ابحثي في VS Code عن: `PORTFOLIO_CONFIG` واضغطي `Ctrl + F`.

### أهم الحاجات اللي محتاجة تعديل

| المكان | المفتاح | الحالة دلوقتي |
|---|---|---|
| الاسم | `personal.name` | Salma Ehsan ✅ |
| الإيميل | `personal.email` | `salmaehsan585@gmail.com` ✅ |
| الموبايل | `personal.phone` | `01201462641` ✅ |
| المكان | `personal.location` | Port Said, Egypt ✅ |
| الأعمال | `portfolio.items` | ✅ 12 عمل بصورها (Branding / Social Media) |
| المهارات | `skills.items` | ✅ |

> **مهم:** بعد أي تعديل اضغطي `Ctrl + S` للحفظ ثم `F5` في المتصفح للمعاينة.

### تغيير صورة
1. حطي الصورة الجديدة داخل `assets/images/`
2. سمّيها بنفس اسم الصورة القديمة (مثلاً `profile.jpg`)
3. موافق على الاستبدال — خلاص، بدون أي تعديل في الكود.

---

## المعاينة على جهازك

أسهل طريقة: افتحي `index.html` بدبل كليك في المتصفح.

> لو الصور مش ظاهرة، شغّلي سيرفر بسيط:
> ```
> npx serve .
> ```
> أو استخدمي إضافة **Live Server** في VS Code.

---

## الرفع على GitHub Pages

### أول مرة (من VS Code)

1. افتحي المجلد في **VS Code**: `File → Open Folder`
2. من الشريط الشمال: **Source Control** (أيقونة الفرع)
3. اكتبي رسالة مثل `Initial portfolio` واضغطي **Commit**
4. اضغطي **Publish Branch** واختاري المستودع
   `salma-ehsan/salmaehsan-portfolio`
5. لو طلب تسجيل دخول، سجّلي بحساب GitHub

### تفعيل الموقع

1. افتحي المستودع على GitHub
2. **Settings → Pages**
3. **Source:** `Deploy from a branch`
4. **Branch:** `main` — **Folder:** `/ (root)`
5. **Save**

بعد دقيقة أو دقيقتين الموقع هيبقى شغّال على:

```
https://salma-ehsan.github.io/salmaehsan-portfolio/
```

---

## ملاحظات

- الموقع Responsive بالكامل (موبايل – تابلت – لابتوب).
- نموذج التواصل بيفتح تطبيق الإيميل عندك وبيجهّز الرسالة جاهزة للإرسال (لأن الموقع Static).
- لتغيير الألوان: افتحي `:root` في أول ملف `index.html`.
  - الخلفية: `--bg-primary: #251836`
  - اللون المميز: `--accent: #F3E0FE`
