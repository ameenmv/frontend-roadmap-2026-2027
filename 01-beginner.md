<div align="center">

<h1>المستوى الأول: Beginner</h1>

<p><strong>HTML · Git & GitHub · CSS · Flexbox · Grid · Responsive · Tailwind</strong></p>

<p>
  <img src="https://img.shields.io/badge/Weeks-1_→_8-EA580C?style=for-the-badge" alt="Weeks 1-8" />
  <img src="https://img.shields.io/badge/Main_Source-Elzero_Web_School-111827?style=for-the-badge" alt="Elzero" />
</p>

</div>

<div dir="rtl">

> **[الرجوع للخريطة](README.md)** · المستوى الأول · [المستوى التاني](02-intermediate.md) · [React](03-react.md) · [Vue](03-vue.md)

---

## الحكاية

في المستوى ده هتبني **الشكل**. هتتعلم إزاي تكتب صفحة ليها معنى (HTML)، وإزاي تخليها حلوة (CSS)، وإزاي تخليها تشتغل على أي شاشة من الموبايل للـ 4K (Responsive)، وإزاي تكتبها أسرع بعشر مرات (Tailwind).

ومن تاني أسبوع، كل حاجة هتعملها هتترفع على **GitHub** وتبقى **Live على النت**. يعني آخر المستوى هيبقى عندك 8 لينكات تقدر تبعتها لأي حد.

| الأسبوع | الموضوع | التاسك |
| :---: | :--- | :--- |
| 1 | [أساسيات HTML](#week-1) | صفحة "عني" |
| 2 | [Semantic HTML و Forms و a11y + Git & GitHub](#week-2) | فورم تسجيل في إيفنت، مرفوع Live |
| 3 | [أساسيات CSS](#week-3) | Profile Card |
| 4 | [Box Model و Position و Flexbox](#week-4) | Navbar + Pricing Cards |
| 5 | [Grid و Transforms و Animations](#week-5) | Dashboard Layout |
| 6 | [Responsive Design و Modern CSS](#week-6) | تحدي من Frontend Mentor |
| 7 | [Tailwind CSS](#week-7) | نفس الـ Pricing بـ Tailwind + Dark Mode |
| 8 | [**مشروع المستوى الأول**](#week-8) | Landing Page كاملة |

---

<a id="week-1"></a>

## الأسبوع 1: أساسيات HTML

**الهدف:** تكتب صفحة HTML كاملة من الصفر، وتفهم كل tag فيها بيعمل إيه.

### المواضيع

- هيكل الصفحة: `<!DOCTYPE>`, `<html>`, `<head>`, `<body>`
- Headings و Paragraphs و Formatting
- Attributes
- Links (`<a>`) والـ Paths (relative vs absolute)
- Images و Lists (`ul`, `ol`, `dl`)
- Tables
- `div` و `span` و HTML Entities

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Learn HTML من #01 لـ #18](https://www.youtube.com/watch?v=6QAELgirvjs&list=PLDoPjvoNmBAw_t_XWUFbBX-c9MafPk9ji&index=1) | ساعتين |
| تكليفات | Elzero: [01-05](https://elzero.org/html-assignments-lesson-from-1-to-5/) · [06-10](https://elzero.org/html-assignments-lesson-from-6-to-10/) · [11-14](https://elzero.org/html-assignments-lesson-from-11-to-14/) · [15-18](https://elzero.org/html-assignments-lesson-from-15-to-18/) | |
| البديل | [Learn HTML - web.dev](https://web.dev/learn/html) | إنجليزي، مقالات |
| مرجع | [HTML Elements Reference - MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element) | |

### التاسك: صفحة "عني"

اعمل صفحة `index.html` عنك إنت، فيها:

- اسمك في `h1`، ونبذة عنك في paragraph
- صورة ليك (أو أي صورة بتعبر عنك) بـ `alt` مكتوب صح
- لستة بالحاجات اللي بتحب تعملها، ولستة مرقمة بأهدافك السنة دي
- جدول بمواعيد مذاكرتك في الأسبوع (الأيام × الوقت × هتذاكر إيه)
- لينكات لأكونتاتك (GitHub, LinkedIn) تفتح في تاب جديدة
- لينك لصفحة تانية `hobbies.html` ولينك يرجعك منها للرئيسية

**ممنوع أي CSS.** الأسبوع ده HTML بس.

**التسليم:** على الداشبورد (الملفات أو لينك).

### تحدي إضافي

اعمل جدول فيه `colspan` و `rowspan`، زي جدول المحاضرات بتاعك في الكلية بالظبط.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين الـ element والـ tag والـ attribute
- [ ] أعرف ليه الـ `alt` مهم في الصور (مش عشان الـ SEO بس)
- [ ] أعرف الفرق بين `./images/me.png` و `/images/me.png` و `../images/me.png`
- [ ] أعرف إمتى أستخدم `ul` وإمتى `ol`
- [ ] أعرف الفرق بين block element و inline element
- [ ] حليت تكليفات Elzero بتاعة الدروس 1 لـ 18

</details>

### أخطاء شائعة

- **إنك تستخدم `<br>` عشان تعمل مسافات.** المسافات شغلة CSS، و `<br>` لسطر جديد جوا نفس الفقرة بس.
- **إنك تختار الـ heading على حسب حجمه.** `h1` لعنوان الصفحة الرئيسي (واحد بس في الصفحة)، و `h2` للأقسام، وهكذا. الحجم بنظبطه بالـ CSS بعدين.
- **إنك تنسى تقفل الـ tags أو تقفلها بالترتيب الغلط** زي `<b><i>text</b></i>`.

> **نصيحة منتور:** متحفظش الـ tags. اكتب كتير وهتحفظها لوحدها. لو نسيت tag، افتح MDN، وده مش عيب. أقدم مبرمج في الدنيا بيعمل كده كل يوم.

---

<a id="week-2"></a>

## الأسبوع 2: Semantic HTML و Forms و Accessibility + Git & GitHub

**الهدف:** تكتب HTML ليه معنى، وتعمل فورم كامل، وترفع شغلك على GitHub ويبقى Live على النت.

### المواضيع

**HTML:**
- Semantic Elements: `header`, `nav`, `main`, `section`, `article`, `aside`, `footer`
- Audio و Video و iFrame
- Forms: كل أنواع الـ inputs، و `label`، و validation attributes (`required`, `pattern`, `min`, `max`)
- مقدمة في الـ Accessibility و ARIA

**Git & GitHub:**
- يعني إيه Version Control، وليه محتاجينه
- `git init`, `add`, `commit`, `push`, `pull`, `clone`
- إنشاء Repo على GitHub وربطه بمشروعك
- **GitHub Pages:** إزاي ترفع موقعك Live مجانًا

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Learn HTML من #19 لـ #37](https://www.youtube.com/watch?v=xlQwlfvrDuI&list=PLDoPjvoNmBAw_t_XWUFbBX-c9MafPk9ji&index=19) | ساعتين |
| تكليفات | Elzero: [19-23](https://elzero.org/html-assignments-lesson-from-19-to-23/) · [24-27](https://elzero.org/html-assignments-lesson-from-24-to-27/) · [28-30](https://elzero.org/html-assignments-lesson-from-28-to-30/) · [31-34](https://elzero.org/html-assignments-lesson-from-31-to-34/) · [35-37](https://elzero.org/html-assignments-lesson-from-35-to-37/) | |
| الأساسي | [Elzero: Learn Git and GitHub من #01 لـ #06](https://www.youtube.com/watch?v=ACOiGZoqC8w&list=PLDoPjvoNmBAw4eOj58MZPakHjaO3frVMF&index=1)، وبعدين [#09](https://www.youtube.com/watch?v=usjh4jj7_nQ&list=PLDoPjvoNmBAw4eOj58MZPakHjaO3frVMF&index=9) | 59 دقيقة |
| مرجع | [Creating a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site) | |
| مرجع | [Web forms - MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/HTML_forms) | |
| مرجع | [Learn Forms - web.dev](https://web.dev/learn/forms) | |

### التاسك: فورم تسجيل في إيفنت CIS

اعمل صفحة تسجيل لإيفنت تقني (Workshop أو Hackathon) فيها:

- `header` فيه اسم الإيفنت و `nav` فيه لينكات للأقسام
- `main` فيه سكشن عن الإيفنت، وسكشن بالـ Agenda (جدول)، وسكشن فيه فيديو أو خريطة المكان (iFrame من Google Maps)
- **فورم تسجيل** فيه: الاسم، والإيميل، والموبايل (`pattern` لرقم مصري 11 رقم)، والكلية (`select`)، والسنة الدراسية (`radio`)، والمجالات المهتم بيها (`checkbox`)، وليه عاوز تحضر (`textarea`)، وزرار Submit
- كل input ليه `label` مربوط بيه صح (`for` و `id`)
- `footer`

وبعدين:
1. اعمل Repo جديد اسمه `cis-event-form`
2. اعمل **3 commits على الأقل** برسايل واضحة (مثلًا: `add event info section`, `add registration form`)
3. فعّل **GitHub Pages** وخلي الصفحة Live

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الصفحة الـ Live.

### تحدي إضافي

افتح الصفحة واقفل الماوس خالص. تقدر تملا الفورم كله وتعمل Submit بالكيبورد بس (`Tab` و `Space` و `Enter`)؟ لو لأ، صلّحها.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف ليه `<nav>` أحسن من `<div class="nav">` حتى لو شكلهم واحد
- [ ] أعرف الفرق بين `GET` و `POST` في الفورم
- [ ] أعرف ليه كل input لازم يبقى ليه `label`
- [ ] أعرف الفرق بين `git add` و `git commit` و `git push`
- [ ] أقدر أعمل Repo جديد وأرفع عليه مشروع من الصفر من غير ما أبص في الفيديو
- [ ] الصفحة بتاعتي Live على GitHub Pages

</details>

### أخطاء شائعة

- **commit واحد اسمه `final` أو `update`.** رسالة الـ commit بتقول **عملت إيه**، وده هيفرق معاك جدًا لما تشتغل مع فريق.
- **إنك ترفع الملفات بالـ Drag & Drop على موقع GitHub.** اتعلم الـ Terminal من دلوقتي، لأنك هتحتاجه كل يوم.
- **إنك تستخدم `placeholder` بدل `label`.** الـ placeholder بيختفي أول ما تكتب، وقارئ الشاشة مش بيعتمد عليه.

> **نصيحة منتور:** GitHub بتاعك هو الـ CV الحقيقي بتاعك. أي شركة هتبص عليه قبل ما تبص على الـ CV. فمن النهارده، كل حاجة بتتعلمها ترفعها، والمربعات الخضرا دي هتفرق معاك جدًا بعد سنة.

---

<a id="week-3"></a>

## الأسبوع 3: أساسيات CSS

**الهدف:** تتحكم في شكل أي عنصر في الصفحة: ألوانه، وخطوطه، ومساحاته، وخلفيته.

### المواضيع

- Syntax و Selectors و Naming Conventions
- Background (color, image, position, size)
- Padding و Margin و Border و Outline
- Display: `block`, `inline`, `inline-block`, `none`
- Width و Height و Overflow
- Text و Typography: fonts، و sizes، و units (`px`, `em`, `rem`, `%`, `vw`)
- Inheritance
- Float (هتفهمه بس، ومش هتستخدمه في الـ layout)
- `calc()` و Opacity

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Learn CSS من #01 لـ #29](https://www.youtube.com/watch?v=X1ulCwyhCVM&list=PLDoPjvoNmBAzjsz06gkzlSrlev53MGIKe&index=1) | 3.5 ساعة |
| تكليفات | Elzero: [01-04](https://elzero.org/css-assignments-lesson-from-1-to-4/) · [05-08](https://elzero.org/css-assignments-lesson-from-5-to-8/) · [09-12](https://elzero.org/css-assignments-lesson-from-9-to-12/) · [13-16](https://elzero.org/css-assignments-lesson-from-13-to-16/) · [17-21](https://elzero.org/css-assignments-lesson-from-17-to-21/) · [22-26](https://elzero.org/css-assignments-lesson-from-22-to-26/) · [27-29](https://elzero.org/css-assignments-lesson-from-27-to-29/) | |
| البديل | [Learn CSS - web.dev](https://web.dev/learn/css) | إنجليزي |
| مرجع | [CSS values and units - MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Values_and_units) | |
| مرجع | [Custom CSS Reset - Josh Comeau](https://www.joshwcomeau.com/css/custom-css-reset/) | هتستخدمه في كل مشروع |

### التاسك: Profile Card

ارجع لصفحة "عني" بتاعة الأسبوع الأول، وحوّلها لـ **Profile Card** في نص الصفحة:

- صورة دايرية، واسمك، ووظيفتك (مثلًا: Frontend Developer in Progress)
- نبذة قصيرة، وأزرار للسوشيال ميديا
- استخدم Google Font
- استخدم `rem` في أحجام الخطوط والمسافات، مش `px`
- ملف CSS منفصل (مفيش `style=""` جوا الـ HTML)
- ارفعها على GitHub وخليها Live

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

خلي الكارت فيه `hover` effect: الكارت يعلى شوية وتظهر تحته shadow أوضح.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين `padding` و `margin`
- [ ] أعرف الفرق بين `em` و `rem`، وإمتى أستخدم كل واحد
- [ ] أعرف الـ Specificity: ليه الـ id بيكسب الـ class
- [ ] أعرف إيه الخصائص اللي بتتورث (inherit) وإيه اللي لأ
- [ ] أقدر أوسّط عنصر أفقيًا بـ `margin: auto`
- [ ] حليت تكليفات Elzero بتاعة الدروس 1 لـ 29

</details>

### أخطاء شائعة

- **إنك تكتب `!important` عشان حاجة مش راضية تتطبق.** دي مشكلة Specificity، فافهمها وحلها صح.
- **إنك تدي `height` ثابت لكل حاجة.** سيب المحتوى يحدد الطول، واستخدم `padding` و `min-height`.
- **أسماء classes زي `red-text` أو `box1`.** سمّي على حسب **الوظيفة** مش الشكل: `card-title`, `profile-image`.

> **نصيحة منتور:** DevTools هو أعز صاحب ليك في CSS. بدل ما تغيّر في الكود وتعمل refresh 50 مرة، غيّر الـ values مباشرة من تاب Elements، ولما توصل للشكل اللي عاوزه، انقله للكود.

---

<a id="week-4"></a>

## الأسبوع 4: Box Model و Position و Flexbox

**الهدف:** تفهم إزاي العناصر بتاخد مساحتها، وتعمل أي layout في اتجاه واحد بـ Flexbox.

### المواضيع

- Position: `static`, `relative`, `absolute`, `fixed`, `sticky`، و `z-index`
- Pseudo Classes (`:hover`, `:focus`, `:nth-child`) و Pseudo Elements (`::before`, `::after`)
- Border Radius و Box Shadow
- **The Box Model** و `box-sizing: border-box`
- Transitions
- Margin Collapse
- **CSS Variables**
- **Flexbox**: كل حاجة في الـ parent والـ child

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Learn CSS من #30 لـ #53](https://www.youtube.com/watch?v=-q5IyjKkKSc&list=PLDoPjvoNmBAzjsz06gkzlSrlev53MGIKe&index=30) | 3.5 ساعة |
| تكليفات | Elzero: [30-33](https://elzero.org/css-assignments-lesson-from-30-to-33/) · [34-37](https://elzero.org/css-assignments-lesson-from-34-to-37) · [38-41](https://elzero.org/css-assignments-lesson-from-38-to-41/) · [42-45](https://elzero.org/css-assignments-lesson-from-42-to-45/) · [46-53](https://elzero.org/css-assignments-lesson-from-46-to-53/) | |
| تدريب | [Flexbox Froggy](https://flexboxfroggy.com/) | خلّص الـ 24 مستوى |
| البديل | [An Interactive Guide to Flexbox - Josh Comeau](https://www.joshwcomeau.com/css/interactive-guide-to-flexbox/) | إنجليزي، تفاعلي، من أحسن الشروحات |
| مرجع | [A Complete Guide to Flexbox - CSS-Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) | اعمله Bookmark |

### التاسك: Navbar + Pricing Cards

اعمل صفحة فيها:

1. **Navbar** ثابت فوق (`sticky`): لوجو على الشمال، ولينكات في النص، وزرار "Sign Up" على اليمين
2. **3 Pricing Cards** جنب بعض (Basic, Pro, Team)، والكارت اللي في النص مميز (أكبر شوية ومكتوب عليه "Most Popular" بـ `::before` أو `position: absolute`)
3. كل كارت فيه: اسم الباقة، والسعر، ولستة مميزات، وزرار
4. كل الألوان والمسافات متعرّفة كـ **CSS Variables** في `:root`
5. الزراير ليها `:hover` و `:focus-visible` بـ `transition`

**ممنوع** `float` أو `position` عشان ترص العناصر جنب بعض. Flexbox بس.

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

غيّر قيمة variable واحد بس (`--primary`)، والصفحة كلها يتغير لونها. ده أساس الـ Theming اللي هتعمله بعدين.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين `relative` و `absolute`، وإن الـ absolute بيتحسب نسبةً لمين
- [ ] أعرف الفرق بين `content-box` و `border-box`
- [ ] أعرف الفرق بين `justify-content` و `align-items`
- [ ] أعرف `flex: 1` معناها إيه بالظبط (grow, shrink, basis)
- [ ] أقدر أوسّط أي حاجة أفقيًا ورأسيًا بـ Flexbox في سطرين
- [ ] خلصت Flexbox Froggy

</details>

### أخطاء شائعة

- **إنك تستخدم `position: absolute` لكل حاجة.** هتلاقي الصفحة باظت أول ما الشاشة تتغير. الـ absolute للحاجات الصغيرة اللي "طايرة" بس، زي badge أو أيقونة.
- **إنك تحط `display: flex` على كل div في الصفحة.** استخدمه لما تكون محتاجه بس.
- **إنك تنسى `box-sizing: border-box`.** حطه في الـ reset في أول كل مشروع وارتاح.

> **نصيحة منتور:** Flexbox هيبقى أكتر حاجة بتستخدمها في حياتك كـ Frontend. افتح Flexbox Froggy مرتين: مرة دلوقتي، ومرة كمان أسبوع من غير ما تبص على الحل.

---

<a id="week-5"></a>

## الأسبوع 5: Grid و Transforms و Animations

**الهدف:** تعمل layouts في اتجاهين بـ Grid، وتخلي الصفحة "حية" بالحركة.

### المواضيع

- Filters و Gradients
- **CSS Grid**: `grid-template-columns`، و `grid-template-areas`، و `gap`، و `minmax()`، و `auto-fill` و `auto-fit`
- 2D و 3D Transforms
- Animations و `@keyframes`
- CSS Selectors بالتفصيل

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Learn CSS من #54 لـ #82](https://www.youtube.com/watch?v=2v9ZhqX6YOk&list=PLDoPjvoNmBAzjsz06gkzlSrlev53MGIKe&index=54) | 4 ساعات |
| تكليفات | Elzero: [54-56](https://elzero.org/css-assignments-lesson-from-54-to-56/) · [57-64](https://elzero.org/css-assignments-lesson-from-57-to-64/) · [65-67](https://elzero.org/css-assignments-lesson-from-65-to-67/) · [68-73](https://elzero.org/css-assignments-lesson-from-68-to-73/) · [74-77](https://elzero.org/css-assignments-lesson-from-74-to-77/) · [78-82](https://elzero.org/css-assignments-lesson-from-78-to-82/) | |
| تدريب | [Grid Garden](https://cssgridgarden.com/) | خلّص الـ 28 مستوى |
| البديل | [An Interactive Guide to CSS Grid - Josh Comeau](https://www.joshwcomeau.com/css/interactive-guide-to-grid/) | إنجليزي، تفاعلي |
| مرجع | [A Complete Guide to CSS Grid - CSS-Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/) | |

### التاسك: Dashboard Layout

اعمل Layout لـ Dashboard (مش لازم يشتغل، شكل بس):

- **Sidebar** على الجنب، و **Header** فوق، و **Main** في النص، باستخدام `grid-template-areas`
- جوا الـ Main: 4 كروت إحصائيات صغيرة فوق، وتحتهم كارت كبير واخد عمودين (مكان chart)، وكارت جنبه للـ "Recent Activity"
- كروت الإحصائيات بتترص لوحدها بـ `repeat(auto-fit, minmax(200px, 1fr))`
- **Loading Spinner** معمول بـ CSS بس (`@keyframes`)
- الكروت ليها hover بـ `transform: translateY()`

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

اعمل **Flip Card**: كارت لما تعمل عليه hover يتقلب ويظهر ضهره (3D Transform + `backface-visibility`).

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف إمتى أستخدم Flexbox وإمتى Grid
- [ ] أعرف `fr` معناها إيه
- [ ] أعرف الفرق بين `auto-fill` و `auto-fit`
- [ ] أعرف الفرق بين `transition` و `animation`
- [ ] أعرف ليه الأحسن أعمل animation على `transform` و `opacity` بدل `top` و `width`
- [ ] خلصت Grid Garden

</details>

### أخطاء شائعة

- **إنك تعمل Grid لكل حاجة أو Flex لكل حاجة.** القاعدة البسيطة: **Grid للـ layout الكبير** (الصفحة)، و **Flex للمكونات الصغيرة** (navbar, buttons).
- **Animations كتير.** الحركة الزيادة بتضايق، وفيه ناس بتتعب منها فعلًا. خليها خفيفة وليها هدف.

> **نصيحة منتور:** لما تشوف موقع عاجبك، افتح DevTools وشوف هو عامل الـ layout إزاي. هتتعلم من ده أكتر من أي كورس.

---

<a id="week-6"></a>

## الأسبوع 6: Responsive Design و Modern CSS

**الهدف:** أي صفحة تعملها تبان صح على الموبايل والتابلت واللابتوب.

### المواضيع

- Media Queries و Breakpoints
- **Mobile First**: تبدأ بالموبايل وتكبّر
- `viewport` meta tag
- Responsive Images (`max-width: 100%`، و `object-fit`)
- `clamp()` للخطوط والمسافات اللي بتكبر لوحدها
- Modern CSS: Container Queries، و `:has()`، و Native CSS Nesting

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Learn CSS من #83 لـ #88](https://www.youtube.com/watch?v=F9FAcVwSV4c&list=PLDoPjvoNmBAzjsz06gkzlSrlev53MGIKe&index=83) | ساعة |
| تكليفات | Elzero: [83-85](https://elzero.org/css-assignments-lesson-from-83-to-85/) · [86-88](https://elzero.org/css-assignments-lesson-from-86-to-88/) | |
| تطبيق | [Elzero: HTML And CSS Template 1](https://www.youtube.com/playlist?list=PLDoPjvoNmBAzHSjcR-HnW9tnxyuye8KbF) | ساعتين |
| مرجع | [Learn Responsive Design - web.dev](https://web.dev/learn/design) | **اقراه**، أهم مرجع في الأسبوع |
| مرجع | [Responsive design - MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Responsive_Design) | |
| مرجع | [Container Queries - MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_containment/Container_queries) | |

> **ملاحظة:** Template 1 ابنيه **مع** Elzero خطوة بخطوة. ده أول مرة تشوف حد بيبني موقع كامل من الصفر، فركّز إزاي بيفكر مش بس بيكتب إيه.

### التاسك: تحدي من Frontend Mentor

1. ادخل على [Frontend Mentor Challenges](https://www.frontendmentor.io/challenges)، واختار Filter: **Free** و **Newbie** أو **Junior**
2. اختار تحدي فيه Mobile و Desktop design
3. ابنيه **Mobile First**
4. ارجع لتاسك الأسبوع 4 (Pricing) والأسبوع 5 (Dashboard) وخليهم Responsive: الكروت تبقى تحت بعض على الموبايل، والـ Sidebar يختفي أو يبقى فوق

**التسليم:** على الداشبورد: 3 لينكات Live (التحدي + Pricing + Dashboard).

### تحدي إضافي

اعمل Card component بيتغير شكله (صورة جنب الكلام أو فوقه) على حسب **مساحة الحاوية** مش حجم الشاشة، باستخدام Container Queries.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف ليه Mobile First أحسن من Desktop First
- [ ] أعرف الـ `viewport` meta tag بيعمل إيه، وإيه اللي بيحصل لو شلته
- [ ] أقدر أستخدم `clamp()` لخط بيكبر ويصغر مع الشاشة
- [ ] أعرف الفرق بين Media Query و Container Query
- [ ] بفتح الـ Device Toolbar في DevTools وأجرب على مقاسات مختلفة

</details>

### أخطاء شائعة

- **إنك تعمل Breakpoint لكل موبايل في السوق.** حط الـ breakpoints في المكان اللي **التصميم بيبوظ فيه**، مش على مقاسات أجهزة معينة.
- **Horizontal scroll على الموبايل.** غالبًا فيه عنصر عرضه ثابت بالـ `px` أو صورة من غير `max-width: 100%`.
- **إنك تجرب في DevTools بس.** افتح اللينك على موبايلك الحقيقي.

> **نصيحة منتور:** أغلب زوار المواقع في مصر جايين من الموبايل مش من اللابتوب. يعني الموبايل مش "نسخة إضافية" من الموقع، هو **الموقع الأساسي**.

---

<a id="week-7"></a>

## الأسبوع 7: Tailwind CSS

**الهدف:** تكتب CSS أسرع بكتير باستخدام Utility Classes، وتفهم ليه أغلب مشاريع React و Vue بتستخدم Tailwind.

### المواضيع

- يعني إيه Utility-First، وليه
- تسطيب Tailwind v4 مع Vite
- Spacing، و Colors، و Typography
- Flexbox و Grid بـ Tailwind
- Responsive: `sm:`، و `md:`، و `lg:`
- States: `hover:`، و `focus:`، و `dark:`
- Customization بـ `@theme`، و `@apply` (وليه متستخدموش كتير)

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Triangles - مثلثات: تعلم Tailwind CSS 4](https://www.youtube.com/playlist?list=PLdnrjoDUmGZ8Q9Dq9ebR9v1xEgqJ6tcfx) | 3.5 ساعة |
| مرجع | [Tailwind CSS Docs: Installation with Vite](https://tailwindcss.com/docs/installation/using-vite) | |
| مرجع | [Styling with utility classes](https://tailwindcss.com/docs/styling-with-utility-classes) | **اقرا الصفحة دي كلها** |

> **ملاحظة مهمة:** Tailwind **مش بديل** إنك تفهم CSS. كل class في Tailwind هو سطر CSS إنت عارفه خلاص. لو مش فاهم `flex justify-between items-center` بتعمل إيه في CSS، ارجع للأسبوع 4.

> **عن Vite:** هتحتاج تسطب [Node.js](https://nodejs.org) (نسخة LTS) عشان تشغّل Vite. متقلقش لو مش فاهم Vite و npm بالظبط دلوقتي، هنشرحهم بالتفصيل في الأسبوع 16. دلوقتي امشي على خطوات الـ installation بس.

### التاسك: Pricing بـ Tailwind + Dark Mode

1. ابني صفحة الـ Navbar + Pricing Cards (تاسك الأسبوع 4) **من الصفر** بـ Tailwind
2. Responsive بالكامل
3. زرار في الـ Navbar بيقلب بين **Light و Dark Mode** (استخدم `dark:`، والـ JS هنا سطرين بس: `document.documentElement.classList.toggle('dark')`)
4. Custom colors في `@theme`

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live (اعمل deploy على [Vercel](https://vercel.com) أو [Netlify](https://www.netlify.com)، لأن GitHub Pages محتاج ظبط زيادة مع Vite).

### تحدي إضافي

قارن حجم ملف الـ CSS النهائي بتاع نسخة Tailwind بحجمه في نسخة CSS العادي. مين أصغر؟ وليه؟

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أقدر أترجم أي class في Tailwind لـ CSS عادي في دماغي
- [ ] أعرف إزاي أسطب Tailwind في مشروع Vite جديد من غير فيديو
- [ ] أعرف `md:flex` معناها "من الـ md وأكبر" مش "على الـ md بس"
- [ ] أعرف إزاي أضيف لون أو font خاص بيا في `@theme`
- [ ] أعرف ليه `@apply` الكتير بيرجعني لنفس مشاكل CSS العادي

</details>

### أخطاء شائعة

- **إنك تتعلم Tailwind قبل ما تفهم CSS.** هتبقى بتحفظ أسماء classes من غير ما تفهم بتعمل إيه.
- **إنك تكتب classes بشكل dynamic** زي `bg-${color}-500`. Tailwind مش هيشوفها ومش هيولّدها.
- **`@apply` في كل حتة.** لو بتعمل كده، إنت بتكتب CSS عادي بطريقة أصعب.

> **نصيحة منتور:** سطّب إضافة **Tailwind CSS IntelliSense** في VS Code. هتوفّرلك نص الوقت اللي بتدوّر فيه على أسماء الـ classes.

---

<a id="week-8"></a>

## الأسبوع 8: مشروع المستوى الأول

**الهدف:** تبني Landing Page حقيقية من تصميم، لوحدك، من غير فيديو تمشي وراه.

ده أول اختبار حقيقي ليك. مفيش كورس الأسبوع ده، **إنت والتصميم بس**.

### المشروع: Landing Page كاملة

اختار تصميم واحد من دول:

- تحدي من [Frontend Mentor](https://www.frontendmentor.io/challenges) مستوى **Junior** أو **Intermediate** (فيه Landing Pages كتير مجانية)
- تصميم Landing Page من [Figma Community](https://www.figma.com/community) (دوّر على `landing page` واختار حاجة فيها Mobile و Desktop)

### المتطلبات

| المتطلب | التفاصيل |
| :--- | :--- |
| **الأقسام** | 5 أقسام على الأقل: Navbar، و Hero، و Features، و Testimonials أو Pricing، و Footer |
| **Responsive** | Mobile First، وشغال صح على 375px و 768px و 1440px |
| **Semantic HTML** | كل قسم في الـ tag الصح، و `h1` واحد بس |
| **Accessibility** | كل الصور ليها `alt`، وكل الزراير شغالة بالكيبورد، والـ contrast مقروء |
| **الأدوات** | CSS عادي أو Tailwind، **إنت تختار** |
| **Git** | 10 commits على الأقل برسايل واضحة، ومفيش commit اسمه `final` |
| **Deploy** | Live على GitHub Pages أو Vercel أو Netlify |
| **README** | صورة للمشروع، ولينك الـ Live، والأدوات اللي استخدمتها، وإيه أصعب حاجة قابلتك |
| **Lighthouse** | افتح DevTools وشغّل Lighthouse، وحاول توصل لـ **90+** في Accessibility و Best Practices |

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live + Screenshot من نتيجة Lighthouse.

### تحدي إضافي

- اعمل نسخة **Dark Mode** للصفحة
- ضيف **Scroll Animations** خفيفة بـ CSS بس (ابحث عن `animation-timeline: view()`)
- لو التصميم جاي من Frontend Mentor، ارفع الحل عندهم واطلب feedback من المجتمع

<details>
<summary><b>Checklist آخر المستوى الأول</b></summary>

<br />

- [ ] أقدر أبني أي صفحة static من تصميم لوحدي
- [ ] بفكر Mobile First من غير ما أفتكر
- [ ] بعرف إمتى أستخدم Flex وإمتى Grid من أول نظرة
- [ ] GitHub بتاعي عليه 8 repos على الأقل، كلهم Live
- [ ] بعرف أقرا تصميم وأطلع منه الألوان والخطوط والمسافات
- [ ] لما حاجة مش ظابطة في CSS، بفتح DevTools وأعرف المشكلة فين

</details>

### أخطاء شائعة

- **إنك تقعد تفتح Template 2 بتاع Elzero وتنسخ منه.** اتفرج لو وقفت في حاجة معينة، بس المشروع لازم يبقى **بتاعك**.
- **إنك تفضّل تظبط Pixel Perfect لحد ما تتعب وتسيبه.** 90% شبه التصميم وشغال صح أحسن من 99% ومش خلصان.
- **إنك تبدأ تكتب كود على طول.** اقعد 20 دقيقة مع التصميم الأول: قسّمه أقسام، وحدد الألوان والخطوط، وارسم الـ Grid/Flex على ورقة.

> **نصيحة منتور:** المشروع ده هيبقى أول حاجة تحطها في الـ Portfolio بتاعك. اعمله كأن حد هيدفعلك فلوس عليه. ولما تخلص، ابعته لحد صاحبك يفتحه من موبايله ويقولك رأيه بصراحة.

---

## خلصت المستوى الأول؟

مبروك. إنت دلوقتي تقدر تبني أي صفحة **ثابتة**. بس الصفحة لسه مش بتتفاعل: الزرار مش بيعمل حاجة، والفورم مش بيتأكد من حاجة، ومفيش داتا بتيجي من أي حتة.

ده بالظبط اللي هنعمله في المستوى الجاي.

**[المستوى التاني: Intermediate (JavaScript و TypeScript)](02-intermediate.md)**

</div>
