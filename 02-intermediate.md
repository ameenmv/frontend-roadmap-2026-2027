<div align="center">

<h1>المستوى التاني: Intermediate</h1>

<p><strong>JavaScript · DOM · Async · APIs · How JS Works · npm & Vite · TypeScript</strong></p>

<p>
  <img src="https://img.shields.io/badge/Weeks-9_→_18-CA8A04?style=for-the-badge" alt="Weeks 9-18" />
  <img src="https://img.shields.io/badge/Main_Source-Elzero_Web_School-111827?style=for-the-badge" alt="Elzero" />
</p>

</div>

<div dir="rtl">

> **[الرجوع للخريطة](README.md)** · [المستوى الأول](01-beginner.md) · المستوى التاني · [React](03-react.md) · [Vue](03-vue.md)

---

## الحكاية

لو HTML هو الهيكل و CSS هو الشكل، فـ **JavaScript هي الروح**.

المستوى ده هو **أهم مستوى في الرودماب كلها**. كل اللي هتعمله في React أو Vue بعد كده هو JavaScript. فلو JS عندك قوية، الـ framework هيبقى سهل جدًا. ولو ضعيفة، هتقضي وقتك كله تايه ومش فاهم الـ error جاي منين.

عشان كده المستوى ده **10 أسابيع**، أطول مستوى في الرودماب، ومفيهوش استعجال.

| الأسبوع | الموضوع | التاسك |
| :---: | :--- | :--- |
| 9 | [أساسيات JavaScript](#week-9) | مجموعة Problems |
| 10 | [Arrays و Loops و Functions و Scope](#week-10) | Grade Calculator |
| 11 | [Higher Order Functions و Objects و Destructuring](#week-11) | تحليل داتا طلبة |
| 12 | [DOM و BOM و Local Storage](#week-12) | Expense Tracker |
| 13 | [Map و Set و Dates و Modules](#week-13) | To-Do App متقسم Modules |
| 14 | [Async JavaScript و Fetch API](#week-14) | Weather App |
| 15 | [إزاي JavaScript شغالة من جوا](#week-15) | Quiz App بالـ Classes |
| 16 | [npm و Vite و Git Branching](#week-16) | نقل المشروع لـ Vite + Pull Requests |
| 17 | [TypeScript](#week-17) | تحويل المشروع لـ TypeScript |
| 18 | [**مشروع المستوى التاني**](#week-18) | أبلكيشن بيكلم API بـ TypeScript |

> **عن كورس Elzero JavaScript:** الكورس 19.5 ساعة في 188 فيديو. هنمشي عليه بالترتيب تقريبًا على مدار 7 أسابيع، وبعدين TypeScript. ومتنساش تكليفات كل جزء على [elzero.org](https://elzero.org/study/javascript-bootcamp-2021-study-plan/).

---

<a id="week-9"></a>

## الأسبوع 9: أساسيات JavaScript

**الهدف:** تكتب برامج صغيرة بـ JS فيها متغيرات وعمليات وشروط، وتعرف تقرا الـ Console.

### المواضيع

- JS بتشتغل فين، وإزاي تربطها بالصفحة (`<script>`، و `defer`)
- Console methods
- Data Types و `typeof`
- `var` vs `let` vs `const`
- Strings و Template Literals
- Operators و Type Coercion
- Numbers و Math Object
- String Methods
- Comparison و Logical Operators
- `if` و ternary و `??` و `switch`

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Learn JavaScript من #001 لـ #039](https://www.youtube.com/watch?v=GM6dQBmc-Xg&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=1) | 4 ساعات |
| تكليفات | Elzero: [01-09](https://elzero.org/javascript-bootcamp-assignments-lesson-from-001-to-009/) · [10-17](https://elzero.org/javascript-bootcamp-assignments-lesson-from-010-to-017/) · [18-22](https://elzero.org/javascript-bootcamp-assignments-lesson-from-018-to-022/) · [23-26](https://elzero.org/javascript-bootcamp-assignments-lesson-from-023-to-026/) · [27-30](https://elzero.org/javascript-bootcamp-assignments-lesson-from-027-to-030/) · [31-32](https://elzero.org/javascript-bootcamp-assignments-lesson-from-031-to-032/) · [33-37](https://elzero.org/javascript-bootcamp-assignments-lesson-from-033-to-037/) · [38-39](https://elzero.org/javascript-bootcamp-assignments-lesson-from-038-to-039/) | |
| البديل | [The Modern JavaScript Tutorial - javascript.info](https://javascript.info) | إنجليزي، **أحسن مرجع مكتوب لـ JS** |
| مرجع | [JavaScript Guide - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide) | |

### التاسك: Problems

اعمل ملف `week-9.js` فيه حل المسائل دي (كل مسألة function منفصلة، واطبع النتيجة في الـ Console):

1. **حاسبة BMI:** تاخد الوزن والطول، وترجع الرقم والتصنيف (نحيف، طبيعي، زيادة، سمنة)
2. **Even or Odd:** رقم، وترجع "زوجي" أو "فردي"، ولو مش رقم ترجع رسالة خطأ
3. **أكبر رقم من 3:** من غير `Math.max`
4. **تحويل درجة الحرارة:** Celsius لـ Fahrenheit والعكس
5. **Grade:** درجة من 100، وترجع التقدير (A, B, C, D, F) بـ `switch`
6. **Palindrome:** كلمة، وترجع `true` لو بتتقري من الناحيتين زي بعض (`level`, `racecar`)
7. **Capitalize:** `"hello world"` تبقى `"Hello World"`

**التسليم:** على الداشبورد: لينك الـ Repo.

### تحدي إضافي

اعمل **لعبة تخمين رقم** بـ `prompt` و `alert`: الكمبيوتر يختار رقم من 1 لـ 100، وإنت تخمن، وهو يقولك "أكبر" أو "أصغر". (هتحتاج loop، فاتفرج على أول فيديو في الـ Loops لو حابب.)

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف ليه `const` هي الـ default، وإمتى أستخدم `let`، وليه منستخدمش `var`
- [ ] أعرف الفرق بين `==` و `===`، وليه دايمًا `===`
- [ ] أعرف ليه `"5" + 3` بتطلع `"53"` و `"5" - 3` بتطلع `2`
- [ ] أعرف الفرق بين `||` و `??`
- [ ] أعرف إيه الـ Falsy Values في JS (فيه 8 منهم)
- [ ] حليت تكليفات Elzero بتاعة الدروس 1 لـ 39

</details>

### أخطاء شائعة

- **إنك تتفرج من غير ما تكتب.** JS بالذات مستحيل تتعلمها بالفرجة. اكتب كل سطر في الفيديو، وغيّر فيه، وبوّظه، وشوف إيه اللي هيحصل.
- **إنك تتجاهل اللون الأحمر في الـ Console.** الـ error مش عدو، دي رسالة بتقولك المشكلة فين بالظبط.

> **نصيحة منتور:** الأسبوع ده هيبان سهل، بس متستعجلش. الـ Type Coercion والـ Falsy Values بالذات هيرجعولك في كل bug غريب هتقابله في حياتك.

---

<a id="week-10"></a>

## الأسبوع 10: Arrays و Loops و Functions و Scope

**الهدف:** تتعامل مع ليستات داتا، وتكرر حاجات، وتقسم الكود لـ functions نضيفة.

### المواضيع

- Arrays: إضافة، وحذف، وبحث، وترتيب، و `slice` vs `splice`
- Loops: `for`، و `for...of`، و `while`، و `break` و `continue`
- Functions: parameters، و `return`، و default و rest parameters
- Anonymous Functions و Arrow Functions
- **Scope:** Global، و Local، و Block، و Lexical

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Learn JavaScript من #040 لـ #070](https://www.youtube.com/watch?v=MLVJhya1CV0&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=40) | 3 ساعات |
| تكليفات | Elzero: [40-47](https://elzero.org/javascript-bootcamp-assignments-lesson-from-040-to-047/) · [48-53](https://elzero.org/javascript-bootcamp-assignments-lesson-from-048-to-053/) · [54-56](https://elzero.org/javascript-bootcamp-assignments-lesson-from-054-to-056/) · [57-63](https://elzero.org/javascript-bootcamp-assignments-lesson-from-057-to-063/) · [64-70](https://elzero.org/javascript-bootcamp-assignments-lesson-from-064-to-070/) | |
| تدريب | [30 Days of JavaScript](https://github.com/Asabeneh/30-Days-Of-JavaScript) (Days 5, 6, 7) | تمارين كتير ومتدرجة |
| مرجع | [javascript.info: Functions](https://javascript.info/function-basics) · [Arrays](https://javascript.info/array) | |

### التاسك: Grade Calculator

اعمل array فيه 10 طلبة، كل طالب array فيه `[name, grade]`. واكتب functions:

1. `getAverage(students)`: متوسط الدرجات
2. `getTopStudent(students)`: أعلى طالب
3. `getFailed(students)`: الطلبة اللي أقل من 50
4. `sortByGrade(students)`: ترتيب تنازلي **من غير ما تغيّر الـ array الأصلي**
5. `printReport(students)`: تطبع تقرير شكله حلو في الـ Console فيه اسم كل طالب ودرجته وتقديره

**ممنوع** `map`، و `filter`، و `reduce` الأسبوع ده (لسه جايين). Loops بس.

**التسليم:** على الداشبورد: لينك الـ Repo.

### تحدي إضافي

اكتب function بتطبع **هرم نجوم** بعدد أدوار تختاره:

```text
    *
   ***
  *****
 *******
```

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين `slice` و `splice`، وأنهي واحدة بتغيّر الـ array الأصلي
- [ ] أعرف الفرق بين `for...of` و `for...in`
- [ ] أعرف الفرق بين function بترجع قيمة وfunction بتطبع
- [ ] أعرف الفرق بين Arrow Function والـ function العادية (في الكتابة على الأقل لحد دلوقتي)
- [ ] أعرف يعني إيه Block Scope، وليه `let` جوا `{}` مش بتتشاف برا

</details>

### أخطاء شائعة

- **function بتعمل 5 حاجات.** كل function تعمل **حاجة واحدة** واسمها يقول هي بتعملها إيه.
- **إنك تنسى `return`.** وبعدين تستغرب ليه النتيجة `undefined`.
- **أسماء متغيرات زي `x`, `arr`, `temp`.** سمّيها `students`, `topStudent`, `averageGrade`.

> **نصيحة منتور:** لو بتكتب نفس الكود مرتين، يبقى المفروض يبقى function.

---

<a id="week-11"></a>

## الأسبوع 11: Higher Order Functions و Objects و Destructuring

**الهدف:** تتعامل مع داتا حقيقية (Array of Objects) بالطريقة اللي بيكتب بيها أي Frontend Developer محترف.

### المواضيع

- **Higher Order Functions:** `map`، و `filter`، و `reduce`، و `forEach`
- **Objects:** إنشاء، و Dot vs Bracket Notation، و Nested Objects
- `this` (مقدمة)
- `Object.create` و `Object.assign`
- **Destructuring:** Arrays، و Objects، و Function Parameters
- **Spread Syntax** `...`

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Learn JavaScript من #071 لـ #085](https://www.youtube.com/watch?v=hTUsHXxEvHc&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=71) | 1.5 ساعة |
| الأساسي | [Elzero: Destructuring من #115 لـ #122](https://www.youtube.com/watch?v=tR6VARwdmzA&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=115)، و[Spread Syntax #132](https://www.youtube.com/watch?v=D9UdBHoAOzg&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=132) | 44 دقيقة |
| تكليفات | Elzero: [71-78](https://elzero.org/javascript-bootcamp-assignments-lesson-from-071-to-078/) · [79-85](https://elzero.org/javascript-bootcamp-assignments-lesson-from-079-to-085/) · [115-122](https://elzero.org/javascript-bootcamp-assignments-lesson-from-115-to-122/) | |
| مرجع | [javascript.info: Array methods](https://javascript.info/array-methods) · [Destructuring](https://javascript.info/destructuring-assignment) | |

### التاسك: تحليل داتا طلبة

خد الـ Array ده (أو اعمل واحد شبهه فيه 15 طالب):

```js
const students = [
  { id: 1, name: "Ahmed", age: 20, track: "frontend", grades: [85, 90, 78], active: true },
  { id: 2, name: "Sara", age: 21, track: "backend", grades: [92, 88, 95], active: true },
  { id: 3, name: "Omar", age: 19, track: "frontend", grades: [60, 45, 70], active: false },
  // ...
];
```

واكتب **من غير أي loop عادي** (`map`، و `filter`، و `reduce` بس):

1. أسماء الطلبة الـ active بس
2. كل طالب ومعاه متوسط درجاته (object جديد فيه `average`)
3. عدد الطلبة في كل track: `{ frontend: 6, backend: 5, ... }` بـ `reduce`
4. أعلى طالب في كل track
5. Function بتاخد `{ name, track }` كـ parameter بـ destructuring وترجع جملة ترحيب
6. ضيف طالب جديد **من غير ما تغيّر الـ array الأصلي** (spread)

**التسليم:** على الداشبورد: لينك الـ Repo.

### تحدي إضافي

اكتب `myMap` و `myFilter` بنفسك: functions بتعمل نفس اللي `map` و `filter` بيعملوه، بس من غير ما تستخدمهم.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين `map` و `forEach` (واحدة بترجع array جديد والتانية لأ)
- [ ] أقدر أكتب `reduce` من غير ما أبص على حاجة
- [ ] أعرف إمتى أستخدم `obj.key` وإمتى `obj[key]`
- [ ] أعرف إن الـ spread بيعمل **shallow copy** بس، وده معناه إيه
- [ ] بقرا كود فيه destructuring ومش بستغربه

</details>

### أخطاء شائعة

- **`map` من غير `return`** في arrow function فيها `{}`. هترجعلك array كله `undefined`.
- **إنك تعدّل في الـ object الأصلي جوا `map`.** المفروض ترجّع object جديد. ده هيبقى **قانون** في React و Vue.

> **نصيحة منتور:** `map`، و `filter`، و `reduce`، والـ destructuring، والـ spread هتكتبهم **كل يوم** في React و Vue. لو الأسبوع ده مش واضح 100%، خد يومين زيادة، وده مش تأخير.

---

<a id="week-12"></a>

## الأسبوع 12: DOM و BOM و Local Storage

**الهدف:** تخلي الصفحة تتفاعل: تضيف وتمسح عناصر، وترد على الضغطات، وتحفظ الداتا حتى لو المستخدم قفل المتصفح.

### المواضيع

- **DOM:** يعني إيه، و Select Elements، و Get/Set Content و Attributes
- Create و Append و Remove Elements
- **Events:** `addEventListener`، و Form Validation، و `preventDefault`
- `classList` و Styling
- DOM Traversing
- **BOM:** `setTimeout` و `setInterval`، و `location`، و `history`، و scroll
- **Local Storage** و Session Storage

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Learn JavaScript من #086 لـ #114](https://www.youtube.com/watch?v=AOabnOI4vOQ&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=86) | 3.5 ساعة |
| تكليفات | Elzero: [86-93](https://elzero.org/javascript-bootcamp-assignments-lesson-from-086-to-093/) · [94-101](https://elzero.org/javascript-bootcamp-assignments-lesson-from-094-to-101/) · [102-110](https://elzero.org/javascript-bootcamp-assignments-lesson-from-102-to-110/) · [111-114](https://elzero.org/javascript-bootcamp-assignments-lesson-from-111-to-114/) | |
| تطبيق | Elzero: [Create Tabs](https://www.youtube.com/watch?v=pnLm4ga_P6k&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=27) · [Image Slider](https://www.youtube.com/watch?v=QmPXb-RHy5s&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=7) · [Countdown Timer](https://www.youtube.com/watch?v=eFsiOTJrrE8&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=16) | اختار واحد وابنيه |
| مرجع | [Introduction to the DOM - MDN](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction) | |
| مرجع | [Window.localStorage - MDN](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage) | |

### التاسك: Expense Tracker

اعمل أبلكيشن لتسجيل المصاريف:

- فورم فيه: الوصف، والمبلغ، والنوع (أكل، مواصلات، كورسات، ...)، والتاريخ
- **Validation:** مفيش حقل فاضي، والمبلغ رقم موجب. اعرض الأخطاء **جوا الصفحة** مش `alert`
- كل مصروف يظهر في لستة، وجنبه زرار حذف
- **إجمالي المصاريف** بيتحدث لوحده
- Filter بالنوع (`select`)
- **كل حاجة بتتحفظ في Local Storage**: اعمل refresh والداتا تفضل موجودة

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

- زرار **Edit** لكل مصروف
- استخدم **Event Delegation**: event listener واحد على اللستة كلها بدل listener لكل زرار

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين `querySelector` و `querySelectorAll`، وإيه اللي بيرجعه كل واحد
- [ ] أعرف الفرق بين `innerHTML` و `textContent`، وليه `innerHTML` ممكن تبقى خطر
- [ ] أعرف يعني إيه Event Delegation، وليه مفيدة
- [ ] أعرف إن Local Storage بيخزن **strings بس**، وإزاي أخزن array أو object
- [ ] أعرف الفرق بين Local Storage و Session Storage

</details>

### أخطاء شائعة

- **إنك تحط داتا المستخدم جوا `innerHTML` من غير تفكير.** لو حد كتب `<img src=x onerror=alert(1)>` في الفورم، هيتنفذ. استخدم `textContent` أو `createElement`.
- **إن الـ UI يبقى هو مصدر الداتا.** خلي عندك **array في JS** هي الأصل، وكل ما تتغير ارسم الـ UI منها من جديد. (ده بالظبط اللي React و Vue بيعملوه.)

> **نصيحة منتور:** لو فهمت فكرة "**الداتا في array، والـ UI بيترسم منها**" الأسبوع ده، يبقى إنت فهمت 50% من React و Vue قبل ما تبدأهم.

---

<a id="week-13"></a>

## الأسبوع 13: Map و Set و Dates و Modules

**الهدف:** تعرف أدوات JS الحديثة، وتقسم الكود بتاعك على ملفات بشكل منظم.

### المواضيع

- **Set** و **Map** (وإمتى تستخدمهم بدل Array و Object)
- WeakSet و WeakMap (مقدمة)
- `Array.from`، و `some`، و `every`
- Date و Time
- Generators (مقدمة، مش هتستخدمها كتير)
- **ES Modules:** `import` و `export`، و Named vs Default

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Map و Set من #123 لـ #133](https://www.youtube.com/watch?v=lsirOGbdWYA&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=123) | 1.5 ساعة |
| الأساسي | [Elzero: Date و Generators و Modules من #159 لـ #168](https://www.youtube.com/watch?v=G5Ql9pQFxJA&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=159) | 51 دقيقة |
| تكليفات | Elzero: [123-133](https://elzero.org/javascript-bootcamp-assignments-lesson-from-123-to-133/) · [159-168](https://elzero.org/javascript-bootcamp-assignments-lesson-from-159-to-168/) | |
| تطبيق | [Elzero: To-Do App With Local Storage](https://www.youtube.com/watch?v=ylsFXMHpFUQ&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=22) | ابنيه، وبعدين اعمل التاسك |
| مرجع | [JavaScript modules - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules) | |

### التاسك: To-Do App متقسم Modules

اعمل To-Do App، بس المرة دي **منظم**:

```text
todo-app/
├── index.html
├── css/style.css
└── js/
    ├── main.js        ← نقطة البداية
    ├── storage.js     ← save و load من Local Storage
    ├── todos.js       ← add, remove, toggle, edit
    └── ui.js          ← رسم اللستة في الصفحة
```

- إضافة، وحذف، وتعليم كـ "خلصت"، وتعديل
- Filters: الكل، و اللي لسه، و اللي خلص
- عدّاد "فاضل X مهام"
- تاريخ إنشاء كل مهمة بشكل مقروء ("من 3 ساعات" أو "13 نوفمبر")
- `<script type="module">`

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

- **Drag & Drop** لترتيب المهام (ابحث عن HTML Drag and Drop API)
- اتفرج على [Regular Expressions من #134 لـ #146](https://www.youtube.com/watch?v=V-8vs_teVlo&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=134) (ساعة)، واعمل validation لعنوان المهمة

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف إمتى أستخدم `Set` (قيم مش متكررة)، وإمتى `Map` (keys من أي نوع)
- [ ] أعرف الفرق بين `export default` و `export`
- [ ] أعرف ليه الـ modules مش بتشتغل لو فتحت الملف بـ double click (لازم Live Server)
- [ ] كل ملف في المشروع عنده مسؤولية واحدة واضحة

</details>

### أخطاء شائعة

- **ملف `main.js` فيه 500 سطر.** لو الملف طويل لدرجة إنك بتعمل scroll كتير عشان تلاقي حاجة، قسّمه.
- **Circular imports:** `a.js` بيعمل import من `b.js` و `b.js` بيعمل import من `a.js`. ده بيعمل مشاكل غريبة.

> **نصيحة منتور:** طريقة تقسيمك للملفات النهارده هي نفس طريقة تقسيم الـ components بكرة في React و Vue. فكّر: "الملف ده مسؤول عن إيه؟"

---

<a id="week-14"></a>

## الأسبوع 14: Async JavaScript و Fetch API

**الهدف:** تجيب داتا حقيقية من الإنترنت وتعرضها في صفحتك.

### المواضيع

- JSON: Parse و Stringify
- يعني إيه API
- Synchronous vs Asynchronous
- **Call Stack، و Web APIs، و Event Loop**
- AJAX و XHR (للفهم بس)
- Callback Hell
- **Promises:** `then`، و `catch`، و `finally`
- **Fetch API**
- `Promise.all`، و `allSettled`، و `race`
- **Async / Await**
- Error Handling بـ `try / catch`

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Learn JavaScript من #169 لـ #188](https://www.youtube.com/watch?v=VA_AROETZ58&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=169) | ساعتين |
| تكليفات | Elzero: [169-178](https://elzero.org/javascript-bootcamp-assignments-lesson-from-169-to-178/) · [179-188](https://elzero.org/javascript-bootcamp-assignments-lesson-from-179-to-188/) | |
| تطبيق | Elzero: [Fetch GitHub Repositories](https://www.youtube.com/watch?v=uCKCSO8vkiU&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=6) · [Currency API](https://www.youtube.com/watch?v=wZ90BnBbRsg&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=4) | |
| مرجع | [Using the Fetch API - MDN](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) | |
| مرجع | [Asynchronous JavaScript - MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Async_JS) | |
| مرجع | [Event loop - javascript.info](https://javascript.info/event-loop) | |

### التاسك: Weather App

اعمل أبلكيشن طقس باستخدام [Open-Meteo API](https://open-meteo.com/) (مجاني ومحتاجش API key):

- Input تكتب فيه اسم مدينة، والأبلكيشن يجيب الإحداثيات من الـ Geocoding API بتاعهم، وبعدين الطقس
- اعرض: درجة الحرارة الحالية، والحالة، والرطوبة، والرياح، وتوقعات الـ 7 أيام الجاية
- **3 حالات لازم تبقى واضحة:** Loading (spinner)، و Error (مدينة مش موجودة أو النت فاصل)، و Success
- `async / await` و `try / catch` (مفيش `.then` الأسبوع ده)
- آخر مدينة دورت عليها تتحفظ في Local Storage وتظهر أول ما تفتح

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

- زرار "**موقعي الحالي**" باستخدام `navigator.geolocation`
- **Debounce** للـ input: متبعتش request مع كل حرف، استنى المستخدم يبطّل كتابة 500ms

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أقدر أشرح الـ Event Loop بالرسم لحد مش فاهمه
- [ ] أعرف ليه `console.log` اللي بعد `setTimeout(fn, 0)` بيطبع الأول
- [ ] أعرف إن `fetch` **مش** بيرمي error لو الـ status كان 404 أو 500، وإزاي أتعامل مع ده (`response.ok`)
- [ ] أعرف الفرق بين `Promise.all` و `Promise.allSettled`
- [ ] أقدر أفتح تاب Network وأشوف الـ request والـ response بتاعه

</details>

### أخطاء شائعة

- **إنك تنسى `await`.** وتلاقي `Promise {<pending>}` بدل الداتا.
- **إنك متتعاملش مع الـ error.** النت هيفصل، والـ API هيقع، والمستخدم هيكتب غلط. الأبلكيشن لازم ميقعش.
- **إنك متعرضش Loading.** المستخدم بيدوس على الزرار ومفيش حاجة بتحصل لمدة ثانيتين، فهيدوس 10 مرات.

> **نصيحة منتور:** Async هو أكتر موضوع بيوقّع الناس في JS. لو حاسس إنك مش فاهم، ده طبيعي جدًا. اتفرج على فيديوهات الـ Event Loop مرتين، وارسمه على ورقة. هيوضح.

---

<a id="week-15"></a>

## الأسبوع 15: إزاي JavaScript شغالة من جوا

**الهدف:** تفهم الحاجات اللي "بتحصل من ورا الستارة": Closures، و `this`، و Prototypes، و Classes. ودي اللي بتتسأل في كل Interview.

### المواضيع

- **OOP:** Constructor Functions و **Classes**
- Static، و Inheritance (`extends`، و `super`)، و Encapsulation (`#private`)
- **Prototypes** و Prototype Chain
- Object Descriptors
- **Closures**
- **`this`** بالتفصيل: في function عادية، وفي arrow function، وفي method، و `call` و `apply` و `bind`
- Hoisting

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: OOP من #147 لـ #158](https://www.youtube.com/watch?v=uv5OULDiCXg&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=147) | ساعة |
| تكليفات | Elzero: [147-158](https://elzero.org/javascript-bootcamp-assignments-lesson-from-147-to-158/) | |
| الأساسي | [Closures - javascript.info](https://javascript.info/closure) | إنجليزي، **لازم تقراه** |
| مرجع | [Closures - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures) · [this - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this) | |
| مرجع | [Inheritance and the prototype chain - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain) | |
| تطبيق | [Elzero: Quiz Application](https://www.youtube.com/watch?v=T5QyLcmcMJ4&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=5) | |

### التاسك: Quiz App بالـ Classes

اعمل أبلكيشن Quiz عن JavaScript (أسئلة إنت كاتبها عن اللي اتعلمته):

- `class Question` (السؤال، والاختيارات، والإجابة الصح، و method `isCorrect(answer)`)
- `class Quiz` (لستة الأسئلة، والسؤال الحالي، والسكور، و methods: `next()`، و `answer()`، و `isFinished()`)
- `class QuizUI` مسؤول عن الرسم بس
- **Timer** لكل سؤال (15 ثانية) معمول بـ **closure**
- شاشة نتيجة في الآخر فيها الإجابات الصح والغلط
- أعلى سكور يتحفظ في Local Storage

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

اعمل function اسمها `createCounter()` بترجع object فيه `increment`، و `decrement`، و `getValue`، والـ count نفسه **مستحيل** يتوصله من برا. (ده Closure، وده سؤال Interview مشهور.)

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أقدر أشرح Closure بمثال من دماغي
- [ ] أعرف `this` بتشاور على إيه في كل حالة من الأربع حالات
- [ ] أعرف ليه الـ arrow functions مش ليها `this` خاص بيها
- [ ] أعرف إن الـ `class` في JS هي syntax أحلى للـ prototypes
- [ ] أعرف يعني إيه Hoisting، والفرق بين `var` و `let` فيه

</details>

### أخطاء شائعة

- **إنك تحفظ تعريف الـ Closure من غير ما تفهمه.** لو مش قادر تكتب مثال من دماغك، يبقى لسه.
- **Class فيها كل حاجة.** نفس قاعدة الـ functions: كل class مسؤولية واحدة.

> **نصيحة منتور:** الأسبوع ده مش هيبان مهم دلوقتي، بس كل Technical Interview لـ Frontend هيسألك في Closures و `this` و Event Loop. ذاكره كويس وارجعله تاني قبل أي interview.

---

<a id="week-16"></a>

## الأسبوع 16: npm و Vite و Git Branching

**الهدف:** تشتغل زي ما الشركات بتشتغل بالظبط: مشروع Vite، و packages من npm، و Branches، و Pull Requests.

### المواضيع

**الأدوات:**
- Node.js و npm: يعني إيه package، و `package.json`، و `dependencies` vs `devDependencies`، و `npm scripts`
- ليه محتاجين Bundler، وإيه هو **Vite**
- `npm create vite@latest`، و `npm run dev`، و `npm run build`
- Environment Variables في Vite (`import.meta.env`)
- **ESLint** و **Prettier**

**Git:**
- Configurations و SSH Keys
- **Branching و Merging**
- **Pull Requests**
- Stash، و Restore، و Reset
- `.gitignore` (ومتنساش `node_modules`)
- Tags و Releases

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Learn Git and GitHub #07 و #08](https://www.youtube.com/watch?v=NWnWIpoFVyU&list=PLDoPjvoNmBAw4eOj58MZPakHjaO3frVMF&index=7)، و[من #10 لـ #20](https://www.youtube.com/watch?v=n43bagVuJPU&list=PLDoPjvoNmBAw4eOj58MZPakHjaO3frVMF&index=10) | 1.5 ساعة |
| تدريب | [Learn Git Branching](https://learngitbranching.js.org/) | تفاعلي، **أحسن طريقة تفهم بيها الـ branches** |
| الأساسي | [Vite: Getting Started](https://vite.dev/guide/) | إنجليزي، قصير |
| مرجع | [About npm](https://docs.npmjs.com/about-npm) | |
| مرجع | [Pro Git Book](https://git-scm.com/book/en/v2) | مرجع كامل ومجاني |

### التاسك: نقل الـ Weather App لـ Vite + Pull Requests

1. اعمل مشروع Vite جديد (Vanilla JS) وانقل فيه الـ Weather App بتاع الأسبوع 14
2. قسّمه modules زي ما عملت في الأسبوع 13
3. سطّب package من npm واستخدمها (مثلًا [`dayjs`](https://www.npmjs.com/package/dayjs) لتنسيق التواريخ)
4. ظبّط ESLint و Prettier
5. **الشغل كله بـ branches:**
   - `main` هو اللي شغال دايمًا
   - كل feature في branch: `feature/vite-setup`، و `feature/forecast-chart`، ...
   - اعمل **Pull Request** لكل branch، واكتب فيه وصف لإنت عملت إيه، واعمله merge
6. Deploy على Vercel أو Netlify، وخلي الـ deploy يحصل **لوحده** مع كل push على `main`

**التسليم:** على الداشبورد: لينك الـ Repo (لازم يبان فيه 3 Pull Requests على الأقل) + لينك الـ Live.

### تحدي إضافي

- خلّص المستويات الـ Main كلها في Learn Git Branching
- اعمل **merge conflict** بإيدك (عدّل نفس السطر في branchين) وحلّه

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف `package.json` فيه إيه، والفرق بين `dependencies` و `devDependencies`
- [ ] أعرف ليه `node_modules` مش بيترفع على GitHub، وإزاي حد تاني يشغّل المشروع
- [ ] أعرف الفرق بين `npm run dev` و `npm run build`
- [ ] أقدر أعمل branch، وأشتغل عليه، وأعمل PR، وأعمل merge
- [ ] أقدر أحل merge conflict بسيط

</details>

### أخطاء شائعة

- **إنك ترفع `node_modules`.** أول سطر في `.gitignore`.
- **إنك ترفع API keys في الكود.** أي حاجة سرية تبقى في `.env`، و `.env` في `.gitignore`. (ومعلومة مهمة: أي حاجة في الـ Frontend، حتى لو في `.env`، **المستخدم يقدر يشوفها**. فمفيش Secret حقيقي في الـ Frontend.)
- **إنك تشتغل على `main` على طول.** حتى لو لوحدك، اتعود على الـ branches.

> **نصيحة منتور:** أول يوم في أي شركة، هيدّوك repo وهيقولولك "اعمل branch وابعت PR". اللي بيعرف يعمل ده من أول يوم بيبان مختلف جدًا.

---

<a id="week-17"></a>

## الأسبوع 17: TypeScript

**الهدف:** تكتب JavaScript بـ Types، فتمسك الأخطاء وإنت بتكتب الكود قبل ما المستخدم يمسكها.

### المواضيع

- يعني إيه TypeScript، وليه الشركات بتستخدمها
- `tsconfig.json` و Strict Mode
- Type Annotations: primitives، و arrays، و functions، و objects
- `any` (وليه منستخدمهاش) و `unknown`
- **Type Aliases** و **Interfaces** (والفرق بينهم)
- Literal Types و **Union** و Intersection
- Tuples، و Enums، و `void`، و `never`
- Type Assertions
- Classes في TS: Access Modifiers، و Abstract Classes
- **Generics**

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Elzero: Learn TypeScript من #01 لـ #38](https://www.youtube.com/watch?v=yUndnE-2osg&list=PLDoPjvoNmBAy532K9M_fjiAmrJ0gkCyLJ&index=1) | 3.5 ساعة |
| تكليفات | Elzero: [01-11](https://elzero.org/typescript-assignments-lessons-from-1-to-11/) · [12-21](https://elzero.org/typescript-assignments-lessons-from-12-to-21/) · [22-31](https://elzero.org/typescript-assignments-lessons-from-22-to-31/) · [32-38](https://elzero.org/typescript-assignments-lessons-from-32-to-38/) | |
| البديل | [Beginners TypeScript - Total TypeScript](https://www.totaltypescript.com/tutorials/beginners-typescript) | إنجليزي، تمارين تفاعلية مجانية |
| مرجع | [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/intro.html) | |
| مرجع | [TypeScript Playground](https://www.typescriptlang.org/play) | جرّب فيه أي حاجة من غير ما تعمل مشروع |

> **ملاحظة:** Elzero بيستخدم `tsc` مباشرة. ده كويس للتعلم، بس في الشغل الحقيقي Vite بيتعامل مع TS لوحده (`npm create vite@latest` واختار **Vanilla + TypeScript**).

### التاسك: تحويل المشروع لـ TypeScript

خد الـ Weather App (نسخة Vite من الأسبوع 16)، وحوّله لـ TypeScript:

- `strict: true` في `tsconfig.json`
- **مفيش ولا `any`** في المشروع كله
- اعمل `interface` أو `type` لكل response جاي من الـ API
- كل function ليها types للـ parameters والـ return
- Generic function واحدة على الأقل (مثلًا `fetchJson<T>(url: string): Promise<T>`)
- `npm run build` يعدّي من غير ولا error

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

استخدم **Discriminated Union** للـ state بتاع الصفحة:

```ts
type State =
  | { status: "idle" }
  | { status: "loading" }
  | { status: "success"; data: Weather }
  | { status: "error"; message: string };
```

وشوف إزاي TS بيمنعك تقرا `data` وإنت في حالة `loading`.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين `type` و `interface`، وإمتى أستخدم كل واحد
- [ ] أعرف الفرق بين `any` و `unknown`
- [ ] أقدر أكتب Generic function بسيطة
- [ ] أعرف إن TypeScript **بتختفي** في الـ build، ومش بتعمل أي حماية وقت التشغيل
- [ ] بقرا الـ error بتاع TS وأفهمه

</details>

### أخطاء شائعة

- **`as any` عشان الـ error يسكت.** إنت كده بتقفل الـ smoke detector عشان صوته عالي.
- **إنك تكتب types لكل حاجة حتى اللي TS عارفها لوحده.** `const name: string = "Ahmed"` مالهاش لازمة. سيب الـ **Type Inference** يشتغل.

> **نصيحة منتور:** أول أسبوع مع TypeScript هتحس إنها بتبطّأك وبتطلعلك errors على الفاضي. بعد أسبوعين هتحس إنك مش قادر تكتب من غيرها. اصبر عليها.

---

<a id="week-18"></a>

## الأسبوع 18: مشروع المستوى التاني

**الهدف:** تبني أبلكيشن كامل بيكلم API حقيقي، بـ TypeScript و Vite، لوحدك.

### المشروع: اختار فكرة

| الفكرة | الـ API | الصعوبة |
| :--- | :--- | :---: |
| **Movies Explorer:** بحث، وتفاصيل فيلم، وقائمة مفضلة | [TMDB API](https://www.themoviedb.org/documentation/api) (محتاج API key مجاني) | متوسط |
| **Countries Explorer:** كل الدول، وبحث، و Filter بالقارة، وصفحة تفاصيل فيها الدول اللي جنبها | [REST Countries](https://restcountries.com/) | متوسط |
| **Mini Store:** منتجات، وبحث، و Filter، و Cart بيتحفظ | [DummyJSON](https://dummyjson.com/) | متوسط+ |
| **GitHub Profile Finder:** بروفايل وrepos وترتيبها وأكتر لغات مستخدمة | [GitHub REST API](https://docs.github.com/en/rest) | متوسط+ |
| **فكرتك إنت** | أي API عام | اتكلم مع المنتور |

### المتطلبات

| المتطلب | التفاصيل |
| :--- | :--- |
| **التقنيات** | Vite + TypeScript (`strict`) + CSS أو Tailwind. **مفيش frameworks** |
| **الصفحات** | صفحة رئيسية فيها لستة + صفحة أو Modal للتفاصيل |
| **البحث والفلترة** | بحث بـ debounce + filter واحد على الأقل |
| **الحالات** | Loading و Error و Empty State ("مفيش نتايج") واضحين |
| **Local Storage** | المفضلة أو الـ Cart أو آخر بحث |
| **التنظيم** | Modules متقسمة صح (`api/`، و `ui/`، و `types/`، و `utils/`) |
| **Responsive** | شغال كويس على الموبايل |
| **Git** | Branches و Pull Requests، ومفيش شغل مباشر على `main` |
| **Deploy** | Vercel أو Netlify، والـ API key (لو فيه) في Environment Variables |
| **README** | صورة، ولينك Live، والتقنيات، وإزاي تشغّله local، وإيه اللي اتعلمته |

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

- **Pagination** أو **Infinite Scroll**
- **URL State:** البحث والفلتر يتحفظوا في الـ URL (`?q=egypt&region=africa`)، فلو بعت اللينك لحد يشوف نفس النتايج
- **Dark Mode** بيتحفظ

<details>
<summary><b>Checklist آخر المستوى التاني</b></summary>

<br />

- [ ] أقدر أبني أبلكيشن تفاعلي كامل بـ JS من غير framework
- [ ] بفهم Async و Promises، ومش بتلخبط فيهم
- [ ] بقسّم الكود modules بشكل منطقي
- [ ] بكتب TypeScript ومش بستخدم `any`
- [ ] بشتغل بـ Git Branches و Pull Requests بشكل طبيعي
- [ ] لما يحصل bug، بعرف أفتح DevTools (Console و Network و Sources) وألاقيه

</details>

### أخطاء شائعة

- **إنك تختار فكرة كبيرة جدًا.** أبلكيشن صغير وكامل وشغال أحسن 100 مرة من أبلكيشن كبير ونصه مش شغال.
- **إنك تكتب كل الكود في الآخر.** اعمل الـ API calls الأول واتأكد إنها شغالة في الـ Console، وبعدين الـ UI.

> **نصيحة منتور:** إنت دلوقتي عارف JavaScript أكتر من ناس كتير بتشتغل React بقالها سنة. ده مش كلام تحفيز، ده لأن أغلب الناس بتقفز على الـ framework على طول. الأساس اللي بنيته ده هو اللي هيفرق معاك في كل حاجة جاية.

---

## خلصت المستوى التاني؟

إنت دلوقتي بتكتب JavaScript و TypeScript وبتبني أبلكيشنز حقيقية. بس أكيد لاحظت إن كل ما المشروع يكبر، تحديث الـ UI بإيدك مع كل تغيير في الداتا بيبقى متعب وملخبط.

ده بالظبط المشكلة اللي React و Vue اتعملوا عشان يحلوها.

**اختار طريقك:**

| [**React**](03-react.md) | [**Vue**](03-vue.md) |
| :---: | :---: |
| React · Router · Redux Toolkit / Zustand · TanStack Query · Testing · **Next.js** | Vue 3 · Vue Router · Pinia · TanStack Query · Testing · **Nuxt** |

مش عارف تختار؟ ارجع لـ [المقارنة في الصفحة الرئيسية](README.md#react-ولا-vue).

</div>
