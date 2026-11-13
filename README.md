<div align="center">

<h1>Frontend Roadmap · 2026–2027</h1>

<p><strong>من أول سطر HTML لحد ما تطلّع أبلكيشن حقيقي على النت</strong></p>

<p>
  <img src="https://img.shields.io/badge/Duration-30_Weeks_+_Week_0-0EA5E9?style=for-the-badge" alt="30 Weeks" />
  <img src="https://img.shields.io/badge/Time-6--8_hrs/week-10B981?style=for-the-badge" alt="6-8 hours per week" />
  <img src="https://img.shields.io/badge/Language-Arabic-F59E0B?style=for-the-badge" alt="Arabic" />
  <img src="https://img.shields.io/badge/Tracks-React_|_Vue-6366F1?style=for-the-badge" alt="React or Vue" />
</p>

<p>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML" />
  <img src="https://img.shields.io/badge/CSS-1572B6?style=flat-square&logo=css&logoColor=white" alt="CSS" />
  <img src="https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/Vue-35495E?style=flat-square&logo=vuedotjs&logoColor=4FC08D" alt="Vue" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/Nuxt-00DC82?style=flat-square&logo=nuxt&logoColor=white" alt="Nuxt" />
</p>

</div>

<div dir="rtl">

---

## الحكاية باختصار

كل موقع بتفتحه، كل زرار بتدوس عليه، كل صفحة بتتحرك قدامك بنعومة، وراها حد اشتغل **Frontend**.

الرودماب دي مش لستة لينكات وخلاص. دي **خطة أسبوع بأسبوع** على مدار سنة دراسية كاملة. كل أسبوع فيه هدف واضح، ومصدر واحد تمشي عليه، وتاسك تسلّمه، وChecklist تقولك إنت فعلاً فهمت ولا لأ.

هتبدأ وإنت مش عارف يعني إيه `<div>`، وهتخلص وعندك على GitHub مشاريع حقيقية **شغالة Live**، ومكتوبة بـ TypeScript و React أو Vue، ومتيستة، ومرفوعة على النت.

> **القاعدة الذهبية:** الفيديو بيعلّمك إن الحاجة موجودة. **الكود اللي بتكتبه بإيدك** هو اللي بيعلّمك إزاي تستخدمها. فلو اتفرجت ساعة، اكتب كود ساعتين.

---

## الخريطة

</div>

```mermaid
flowchart TD
    W0["Week 0 · Setup & How the Web Works"] --> B

    subgraph B["Level 1 · Beginner · Weeks 1-8"]
        direction LR
        B1["HTML"] --> B2["Git & GitHub"] --> B3["CSS"] --> B4["Flexbox · Grid"] --> B5["Responsive"] --> B6["Tailwind"]
    end

    B --> BP{{"Project 1 · Landing Page"}}
    BP --> I

    subgraph I["Level 2 · Intermediate · Weeks 9-18"]
        direction LR
        I1["JS Basics"] --> I2["Functions · Arrays · Objects"] --> I3["DOM"] --> I4["Async · APIs"] --> I5["How JS Works"] --> I6["Tooling"] --> I7["TypeScript"]
    end

    I --> IP{{"Project 2 · API App with TS"}}
    IP --> CHOOSE{"Choose your framework"}

    CHOOSE --> R
    CHOOSE --> V

    subgraph R["Level 3 · React · Weeks 19-30"]
        direction LR
        R1["Components · State"] --> R2["Router"] --> R3["Redux Toolkit / Zustand"] --> R4["TanStack Query"] --> R5["Testing · Perf · a11y"] --> R6["Next.js"]
    end

    subgraph V["Level 3 · Vue · Weeks 19-30"]
        direction LR
        V1["Components · Reactivity"] --> V2["Vue Router"] --> V3["Pinia"] --> V4["TanStack Query"] --> V5["Testing · Perf · a11y"] --> V6["Nuxt"]
    end

    R --> F{{"Final Project"}}
    V --> F

    classDef zero fill:#0f172a,stroke:#64748b,color:#ffffff
    classDef beg fill:#fff7ed,stroke:#ea580c,color:#7c2d12
    classDef mid fill:#fefce8,stroke:#ca8a04,color:#713f12
    classDef react fill:#ecfeff,stroke:#0891b2,color:#164e63
    classDef vue fill:#ecfdf5,stroke:#059669,color:#064e3b
    classDef proj fill:#ede9fe,stroke:#7c3aed,color:#4c1d95
    class W0,CHOOSE zero
    class B1,B2,B3,B4,B5,B6 beg
    class I1,I2,I3,I4,I5,I6,I7 mid
    class R1,R2,R3,R4,R5,R6 react
    class V1,V2,V3,V4,V5,V6 vue
    class BP,IP,F proj
```

<div dir="rtl">

---

## المستويات

| المستوى | الأسابيع | هتتعلم إيه | هتخرج بإيه |
| :--- | :---: | :--- | :--- |
| **[Week 0: التمهيد](#week-0)** | 0 | النت بيشتغل إزاي، تجهيز الجهاز، إزاي تذاكر وتسأل صح | جهاز جاهز ودماغ فاهمة اللعبة ماشية إزاي |
| **[المستوى الأول: Beginner](01-beginner.md)** | 1 - 8 | HTML · Git & GitHub · CSS · Flexbox · Grid · Responsive · Tailwind | Landing Page Responsive مرفوعة Live |
| **[المستوى التاني: Intermediate](02-intermediate.md)** | 9 - 18 | JavaScript من الصفر · DOM · Async · APIs · إزاي JS شغالة من جوا · npm و Vite · TypeScript | أبلكيشن بيكلم API ومكتوب بـ TypeScript |
| **[المستوى التالت: React](03-react.md)** | 19 - 30 | React · Router · State Management · TanStack Query · Testing · Performance · a11y · Next.js | مشروع تخرج كامل بـ Next.js |
| **[المستوى التالت: Vue](03-vue.md)** | 19 - 30 | Vue 3 · Vue Router · Pinia · TanStack Query · Testing · Performance · a11y · Nuxt | مشروع تخرج كامل بـ Nuxt |

### React ولا Vue؟

الاتنين ممتازين، والأهم إنك **تختار واحد وتكمّل فيه**، ومتنطّش بينهم.

| | React | Vue |
| :--- | :--- | :--- |
| **سوق الشغل** | الأكثر طلبًا في مصر والخليج وبرا | مطلوب، خصوصًا مع شركات Laravel وفي آسيا وأوروبا |
| **منحنى التعلم** | محتاج JavaScript قوية لأن كل حاجة JS | أسهل في البداية، والـ template قريب من HTML |
| **الـ Ecosystem** | ضخم جدًا، وكل مشكلة ليها 10 حلول | أصغر بس منظم، وأغلب الأدوات رسمية |
| **الـ Meta-framework** | Next.js | Nuxt |
| **اختاره لو** | عاوز أكبر عدد فرص | عاوز تجربة أنضف وأسرع في البداية، أو شغال مع Laravel |

> مش متأكد؟ **اختار React.** ولو حبيت Vue بعدين، هتتعلمه في أسبوعين لأن المفاهيم واحدة.

---

## شكل كل أسبوع

كل أسبوع في الرودماب ماشي بنفس الترتيب، فهتتعود عليه بسرعة:

| الجزء | يعني إيه |
| :--- | :--- |
| **الهدف** | جملة واحدة: آخر الأسبوع هتكون قادر تعمل إيه |
| **المواضيع** | الكلام اللي هيتشرح |
| **المصادر** | **مصدر أساسي** تمشي عليه (عربي غالبًا)، و**بديل** لو مرتحتش للأساسي، و**مرجع** ترجعله وقت ما تحتاج |
| **التاسك** | الحاجة اللي **لازم** تعملها وتسلّمها على الداشبورد |
| **تحدي إضافي** | لو خلصت بدري وعاوز تزوّد، وده مش إجباري |
| **Checklist آخر الأسبوع** | أسئلة تسألها لنفسك؛ لو جاوبت عليها كلها من غير ما تبص، تبقى خلصت الأسبوع |
| **أخطاء شائعة** | الغلطات اللي كل الناس بتقع فيها، عشان متقعش فيها إنت كمان |
| **نصيحة منتور** | حاجة اتعلمناها بالطريقة الصعبة |

### توزيع الـ 6-8 ساعات في الأسبوع

ده اقتراح، مش قانون:

| اليوم | تعمل إيه | الوقت |
| :--- | :--- | :---: |
| يوم 1 | فيديوهات + كتابة كل كود في الفيديو بإيدك | 1.5 - 2 ساعة |
| يوم 2 | باقي الفيديوهات + تكليفات Elzero لو موجودة | 1.5 - 2 ساعة |
| يوم 3 | قراءة المرجع (MDN / Docs) في الحاجات اللي مكانتش واضحة | ساعة |
| يوم 4 | التاسك | 1.5 - 2 ساعة |
| يوم 5 | تكملة التاسك + الـ Checklist + رفع على GitHub والتسليم | ساعة |

> **مدة الفيديوهات:** جنب كل مصدر هتلاقي مدته الحقيقية. لو فيديوهات الأسبوع أكتر من 3.5 ساعة، اتفرج بسرعة **1.25x**، ولو حاجة مش واضحة رجّعها بالسرعة العادية.

> **تكليفات Elzero:** كورسات Elzero ليها تكليفات على [elzero.org](https://elzero.org) لكل مجموعة دروس، وهتلاقي لينكها في كل أسبوع. حلها **قبل** التاسك، لأنها التسخين.

---

## الـ AI في الرودماب دي

الـ AI (ChatGPT, Claude, Copilot, Cursor...) أداة قوية جدًا، بس لو استخدمتها غلط في الأول **هتطلع مبرمج مش عارف يكتب سطر لوحده**. عشان كده عندنا قواعد بتتغير مع كل مستوى:

| المستوى | المسموح | الممنوع |
| :--- | :--- | :--- |
| **Beginner** | تسأله "يعني إيه X؟" أو "اشرحلي الفرق بين X و Y" زي ما تسأل مدرس | إنه يكتبلك كود. اقفل الـ Copilot والـ autocomplete بتاع الـ AI في VS Code خالص |
| **Intermediate** | تديله الكود **بتاعك** ويقولك الغلط فين، وتطلب منه يشرحلك error | إنه يكتب حل التاسك. لو كتبلك كود، اقفله واكتبه إنت من دماغك |
| **Advanced** | تستخدمه كأداة شغل: يكتب boilerplate، ويقترح tests، ويعمل review للكود بتاعك. فيه أسبوع كامل عن إزاي تشتغل معاه زي الـ Pro | إنك تسلّم كود مش فاهم كل سطر فيه. لو المنتور سألك "السطر ده بيعمل إيه؟" ومعرفتش، يبقى التاسك مرفوض |

> **الاختبار البسيط:** لو قفلنا النت دلوقتي، تقدر تكتب الكود ده تاني؟ لو الإجابة لأ، يبقى إنت لسه متعلمتوش.

---

<a id="week-0"></a>

## Week 0: التمهيد

**الهدف:** تفهم إيه اللي بيحصل لما تكتب `google.com` في المتصفح، ويبقى جهازك جاهز تكتب عليه كود.

الأسبوع ده مش محسوب من الـ 30، وهو اللي بيفرق بين حد بيحفظ وحد فاهم.

### المواضيع

- يعني إيه Frontend و Backend و Full Stack، وإيه دور كل واحد
- الإنترنت شغال إزاي: Client و Server، و HTTP، و DNS، و IP
- إيه اللي بيحصل من ساعة ما تكتب URL لحد ما الصفحة تظهر
- المتصفح بيعمل إيه بالـ HTML و CSS و JS
- تسطيب وتظبيط VS Code
- أساسيات الـ Terminal: `cd`, `ls`, `mkdir`, `touch`
- Chrome DevTools: Elements و Console و Network
- إزاي تذاكر صح، وإزاي تسأل سؤال تقني كويس

### المصادر

| النوع | المصدر | ملاحظات |
| :--- | :--- | :--- |
| الأساسي | [كيف يعمل الإنترنت؟ - غريب الشيخ](https://www.youtube.com/watch?v=TnMNDQHB33Q) | 13 دقيقة |
| الأساسي | [شرح DNS بالعربي - IT Dose](https://www.youtube.com/watch?v=s-9143t3cHA) | 7 دقايق |
| إضافي | [What happens when you type a URL into your browser? - ByteByteGo](https://www.youtube.com/watch?v=AlkDbnbv7dk) | 5 دقايق، إنجليزي بس الرسومات بتوضح كل حاجة |
| الأساسي | [الفرق بين Front end و Back end - أحمد محمود](https://www.youtube.com/watch?v=vwvPFuh7ZDs) | 7 دقايق |
| الأساسي | [حوّل VS Code زي المحترفين - غريب الشيخ](https://www.youtube.com/watch?v=0u53L0GaPFc) | 12 دقيقة |
| الأساسي | [Learn Command Line - Elzero](https://www.youtube.com/playlist?list=PLDoPjvoNmBAxzNO8ixW83Sf8FnLy_MkUT) | ساعة |
| الأساسي | [استخدام Chrome DevTools - Elzero](https://www.youtube.com/watch?v=_IKTGQosYMo) | 12 دقيقة |
| مرجع | [How the web works - MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development/Getting_started/Web_standards/How_the_web_works) | مقال قصير |
| مرجع | [An overview of HTTP - MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview) | ارجعله لما تيجي في Async |
| مرجع | [Chrome DevTools Overview](https://developer.chrome.com/docs/devtools/overview) | |

### التاسك

1. سطّب **VS Code** و **Google Chrome** (أو أي متصفح Chromium) و **Git**.
2. سطّب الإضافات دي في VS Code: `Live Server`، و `Prettier`، و `Error Lens`، و `Auto Rename Tag`.
3. اعمل أكونت على **[GitHub](https://github.com)** بإيميل حقيقي، واسم احترافي (`ahmed-ali` مش `a7med_elgamed_2005`).
4. اكتب في ملف `week-0.md` إجابتك **بأسلوبك** على السؤال ده: "إيه اللي بيحصل من ساعة ما أكتب `facebook.com` لحد ما الصفحة تظهر؟" (من 10 لـ 15 سطر، و ممنوع تنسخ من AI).
5. افتح أي موقع بتحبه، وافتح DevTools، وغيّر أي نص في الصفحة من تاب Elements، وخد Screenshot.

**التسليم:** على الداشبورد: لينك أكونت GitHub + الملف + الـ Screenshot.

### تحدي إضافي

افتح تاب **Network** في DevTools واعمل Refresh لأي موقع. اكتب: كام Request اتبعتوا؟ وإيه أكبر ملف اتحمّل؟ وإيه أنواع الملفات اللي شفتها (HTML, CSS, JS, Images, Fonts)؟

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أقدر أشرح الفرق بين Frontend و Backend لحد مش بتاع برمجة
- [ ] أعرف يعني إيه Client و Server و Request و Response
- [ ] أعرف الـ DNS بيعمل إيه، وليه محتاجينه
- [ ] أقدر أفتح Terminal وأتنقل بين الفولدرات وأعمل فولدر جديد
- [ ] أقدر أفتح DevTools وأعدّل في الصفحة وأشوف الـ Console
- [ ] VS Code متسطب ومتظبط، و Live Server شغال

</details>

### أخطاء شائعة

- **إنك تقعد أسبوعين تختار أحسن Theme وأحسن Font لـ VS Code.** الأدوات مش هي اللي بتعلّمك. ظبّط الأساسي وابدأ.
- **إنك تسطب 40 Extension.** كل إضافة زيادة بتبطّأ المحرر وبتخبّي عنك حاجات المفروض تتعلمها.
- **إنك تفتكر الأسبوع ده "مش مهم".** كل مشكلة هتقابلك في الـ Async والـ APIs بعد كده أصلها في الأسبوع ده.

### إزاي تسأل سؤال تقني صح

لما تقف في حاجة، قبل ما تسأل المنتور أو الجروب:

1. **اقرا الـ Error كويس.** 80% من الوقت الحل مكتوب في رسالة الخطأ.
2. **ادوّر بالـ Error نفسه** على Google.
3. **جرّب حاجة لمدة 20-30 دقيقة.** لو فضلت واقف، اسأل، ومتقعدش 3 أيام واقف.
4. لما تسأل، قول: **كنت عاوز أعمل إيه** + **عملت إيه** + **حصل إيه** + **الكود والـ Error كـ text مش صورة موبايل للشاشة**.

> **نصيحة منتور:** أكتر حاجة بتفرق بين اللي بيكمّل واللي بيقف في النص هي **الاستمرارية** مش الذكاء. ساعة كل يوم أحسن من 7 ساعات يوم الجمعة. ولو فوّت أسبوع، متبدأش من الأول. كمّل من مكانك.

---

## أسئلة بتتكرر

<details>
<summary><b>محتاج لابتوب قوي؟</b></summary>

<br />

لأ. أي جهاز عليه 8GB RAM يكفي لحد آخر الرودماب. لو 4GB هيمشي في الـ Beginner والـ Intermediate، وهيتقل شوية مع React/Vue بس هيمشي.

</details>

<details>
<summary><b>لازم أكون شاطر في الماث؟</b></summary>

<br />

لأ. الـ Frontend محتاج **تفكير منطقي** أكتر من ماث. لو بتعرف تحل مسألة خطوة بخطوة، يبقى إنت تمام.

</details>

<details>
<summary><b>الإنجليزي بتاعي ضعيف، هينفع؟</b></summary>

<br />

أيوه، وعشان كده أغلب المصادر الأساسية عربي. بس مع الوقت هتلاقي نفسك محتاج تقرا Docs إنجليزي، وده طبيعي. ابدأ بالـ Docs من أول المستوى التاني، ولو مفهمتش جملة ترجمها. بعد شهرين هتلاقي نفسك بتقرا عادي.

</details>

<details>
<summary><b>فاتني أسبوع أو اتنين، أعمل إيه؟</b></summary>

<br />

متقلقش ومتبدأش من الأول. ركّز على **التاسك** و**الـ Checklist** بتوع الأسابيع اللي فاتتك، وسيب التحديات الإضافية. وكلّم المنتور بتاعك.

</details>

<details>
<summary><b>ليه مفيش Bootstrap أو SASS؟</b></summary>

<br />

لأن الـ CSS الحديث بقى فيه variables و nesting، فـ SASS بقى أقل أهمية بكتير. و Tailwind أخد مكان Bootstrap في أغلب المشاريع الجديدة، خصوصًا مع React و Vue. لو اشتغلت في شركة بتستخدمهم، هتتعلمهم في يومين لأنك فاهم CSS كويس.

</details>

<details>
<summary><b>ليه TypeScript قبل React/Vue مش بعدهم؟</b></summary>

<br />

لأن أغلب الشركات النهارده بتكتب React و Vue بـ TypeScript. فبدل ما تتعلم الـ framework بـ JS وبعدين تتعلمه تاني بـ TS، هتدخله وإنت بتكتب TS من أول يوم، زي الشغل الحقيقي بالظبط.

</details>

---

## إيه الجديد عن رودماب 2025-2026؟

| 2025-2026 | 2026-2027 |
| :--- | :--- |
| لستة لينكات مقسمة بالمواضيع | خطة **أسبوع بأسبوع** بمدة ومصدر أساسي وتاسك |
| مفيش تاسكات ولا مشاريع إلزامية | تاسك كل أسبوع + **3 مشاريع كبيرة** |
| إنجليزي | **عربي** |
| Webpack، و Bootstrap، و SASS، و Recoil، و MobX | **Vite**، و **Tailwind v4**، و **Zustand / Redux Toolkit**، و **Pinia** |
| TypeScript في الآخر كـ Advanced | **TypeScript قبل الـ framework** |
| مفيش Next.js ولا Nuxt | **أسبوعين** لـ Next.js أو Nuxt |
| مفيش كلام عن الـ AI | **سياسة AI متدرجة** + أسبوع عن الشغل معاه |

الرودماب القديمة لسه موجودة لو حبيت ترجعلها: [2025-2026 Frontend Roadmap](https://github.com/CIS-Team/2025-2026-Roadmaps/tree/main/Frontend)

---

## ابدأ دلوقتي

1. خلّص [Week 0](#week-0)
2. افتح [المستوى الأول: Beginner](01-beginner.md)
3. ومتنساش: **اكتب كود كل يوم**

</div>

---

<div align="center">

**Maintained by [Ameen MV](https://github.com/ameenmv)** · Frontend Mentor @ CIS Team

[![GitHub](https://img.shields.io/badge/GitHub-%2312100E.svg?&style=for-the-badge&logo=Github&logoColor=white)](https://github.com/ameenmv)
[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ameeenmv)
[![Instagram](https://img.shields.io/static/v1?message=Instagram&logo=instagram&label=&color=E4405F&logoColor=white&labelColor=&style=for-the-badge)](https://www.instagram.com/ameeen_mv)
[![Twitter](https://img.shields.io/badge/twitter-%231DA1F2.svg?&style=for-the-badge&logo=twitter&logoColor=white)](https://x.com/ameeen_mv)
[![Gmail](https://img.shields.io/badge/gmail-%23D14836.svg?&style=for-the-badge&logo=gmail&logoColor=white)](mailto:ameeenmv@gmail.com)

[All CIS Team Tracks](https://github.com/CIS-Team/2026-2027-Roadmaps)

</div>
