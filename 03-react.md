<div align="center">

<h1>المستوى التالت: React</h1>

<p><strong>React · Router · State Management · TanStack Query · Testing · Performance · a11y · Next.js</strong></p>

<p>
  <img src="https://img.shields.io/badge/Weeks-19_→_30-0891B2?style=for-the-badge" alt="Weeks 19-30" />
  <img src="https://img.shields.io/badge/React-19-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React 19" />
  <img src="https://img.shields.io/badge/Next.js-App_Router-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" />
</p>

</div>

<div dir="rtl">

> **[الرجوع للخريطة](README.md)** · [المستوى الأول](01-beginner.md) · [المستوى التاني](02-intermediate.md) · React · [Vue](03-vue.md)

---

## الحكاية

فاكر في الأسبوع 12 لما كنت بتحدّث الـ UI بإيدك كل ما الداتا تتغير؟ React بتقولك: **إنت قولّي الـ UI شكله إيه لما الداتا تبقى كده، وأنا هتصرف.**

في المستوى ده هتتعلم React، وبعدين الأدوات اللي أي مشروع React حقيقي بيستخدمها، وفي الآخر **Next.js** اللي بيحوّل React من مكتبة لـ framework كامل.

| الأسبوع | الموضوع | التاسك |
| :---: | :--- | :--- |
| 19 | [Components و JSX و Props](#week-19) | تحويل Landing Page لـ Components |
| 20 | [State و Events و Forms](#week-20) | Multi-step Form |
| 21 | [Context و useEffect و Data Fetching](#week-21) | Movies App (نسخة React) |
| 22 | [React Router](#week-22) | أبلكيشن متعدد الصفحات |
| 23 | [Styling و Component Libraries](#week-23) | UI Kit صغير بـ Tailwind + shadcn/ui |
| 24 | [State Management](#week-24) | Shopping Cart |
| 25 | [TanStack Query](#week-25) | Dashboard بـ Server State |
| 26 | [Testing](#week-26) | Tests للـ Cart |
| 27 | [Performance و Accessibility](#week-27) | Audit وتحسين مشروع |
| 28 | [Next.js: الأساسيات والـ Routing](#week-28) | Blog بـ Next.js |
| 29 | [Next.js: Data و SEO و Deploy + الشغل مع الـ AI](#week-29) | تكملة الـ Blog + Deploy |
| 30 | [**مشروع التخرج**](#week-30) | أبلكيشن كامل |

> **قبل ما تبدأ:** المصدر العربي الأساسي في أغلب المستوى ده هو [كورس رياكت - أكاديمية ترميز](https://www.youtube.com/playlist?list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS). الكورس فيه أكتر من 120 درس، ومليان تحديات وحلولها. ولو في أي وقت حسيت إن الشرح فيه حاجة قديمة، **[react.dev](https://react.dev/learn)** هو المرجع الرسمي (وفيه [نسخة عربي](https://ar.react.dev/learn)).

> **عن TypeScript:** من النهارده، **كل مشروع React هتعمله بـ TypeScript**. الكورسات أغلبها بـ JS، فدي فرصتك تتدرب: اتفرج بـ JS واكتب بـ TS. ولما تقف، افتح [React with TypeScript](https://react.dev/learn/typescript).

---

<a id="week-19"></a>

## الأسبوع 19: Components و JSX و Props

**الهدف:** تفكر بطريقة React: كل حاجة في الصفحة component، والـ components بتتكلم مع بعض بالـ props.

### المواضيع

- يعني إيه React، وليه موجودة
- إنشاء مشروع بـ Vite (`npm create vite@latest` واختار React + TypeScript)
- هيكل المشروع
- **Components** و **JSX**
- Styles و Classes في JSX
- **Props**، و `children`
- Conditional Rendering
- Rendering Lists و `key`

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [ترميز: كورس رياكت من الدرس 1 لـ 20](https://www.youtube.com/watch?v=T9DTxrQ1BU0&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=3) | 4 ساعات |
| البديل | [Yehia Tech: أساسيات رياكت في 90 دقيقة](https://www.youtube.com/playlist?list=PL8q8h6vqfkSVeuw14BwrtJRIg3tAwq0ds) | مراجعة سريعة لكل اللي فوق |
| مرجع | [Quick Start - react.dev](https://react.dev/learn) | |
| مرجع | [Thinking in React - react.dev](https://react.dev/learn/thinking-in-react) | **أهم صفحة في الأسبوع** |

> لو الكورس عمل المشروع بـ `create-react-app`، **استخدم Vite بدلها**. `create-react-app` اتوقف ومبقاش حد بيستخدمه.

### التاسك: تحويل Landing Page لـ Components

خد مشروع الـ Landing Page بتاع الأسبوع 8، وحوّله لـ React + TypeScript:

- قسّم الصفحة: `Navbar`، و `Hero`، و `Features`، و `FeatureCard`، و `Testimonials`، و `Footer`، ...
- أي حاجة متكررة (كروت، testimonials، لينكات الـ navbar) تبقى **array of objects** وتترسم بـ `map`
- كل component ليه `Props` type واضح
- مفيش component أكبر من 80 سطر تقريبًا

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

اعمل component اسمه `Button` بياخد `variant` (`"primary" | "secondary" | "ghost"`) و `size` (`"sm" | "md" | "lg"`)، واستخدمه في الصفحة كلها.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف إن JSX مش HTML، وأعرف الفروق (`className`، و `htmlFor`، و `{}`، و self-closing)
- [ ] أعرف ليه الـ `key` مهم في الـ lists، وليه مينفعش أستخدم الـ index في كل الحالات
- [ ] أعرف إن الـ props **read-only**، ومينفعش الـ component يغيّرها
- [ ] أقدر أبص على تصميم وأقسّمه components في دماغي
- [ ] أعرف `children` بتستخدم في إيه

</details>

### أخطاء شائعة

- **component واحد اسمه `App` فيه الصفحة كلها.** قسّم.
- **إنك تنسى `key` أو تحط `Math.random()`.** الـ key لازم يبقى ثابت ومميز، زي `id`.
- **إنك تعمل الـ component الجديد جوا component تاني.** كل component يتعرّف برا، في ملفه.

> **نصيحة منتور:** اقرا صفحة **Thinking in React** مرتين. الصفحة دي لوحدها بتفرق بين حد بيكتب React وحد فاهم React.

---

<a id="week-20"></a>

## الأسبوع 20: State و Events و Forms

**الهدف:** تخلي الـ components تفتكر حاجات وتتغير لما المستخدم يتفاعل.

### المواضيع

- يعني إيه State، وليه المتغير العادي مش بيكفي
- إزاي React بيعمل re-render (Virtual DOM)
- **`useState`**
- Events و Event Handlers
- **Forms:** Controlled Inputs، و Select و Radio و Checkbox
- **Immutability:** تحديث Objects و Arrays في الـ State صح
- Updater function: `setCount(c => c + 1)`

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [ترميز: كورس رياكت من الدرس 21 لـ 40](https://www.youtube.com/watch?v=rnVI3UKcKQA&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=25) | 3.5 ساعة |
| تطبيق | [ترميز: المشروع الأول، Loan Application Form (الدروس 41 لـ 43)](https://www.youtube.com/watch?v=hFrOluMFZxA&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=45) | 1.5 ساعة، **اختياري** لو التاسك واخد وقتك |
| مرجع | [Adding Interactivity - react.dev](https://react.dev/learn/adding-interactivity) | |

> كورس ترميز فيه **تحدي بعد كل جزء، وبعده فيديو الحل**. حل التحدي بنفسك الأول، وبعدين اتفرج على الحل. ولو حليته صح، تقدر تتفرج على الحل بسرعة 1.5x.
| مرجع | [Managing State - react.dev](https://react.dev/learn/managing-state) | |

### التاسك: Multi-step Form

اعمل فورم تسجيل على 3 خطوات (زي فورم التقديم على كورس):

1. **البيانات الشخصية:** الاسم، والإيميل، والموبايل
2. **البيانات الأكاديمية:** الكلية، والسنة، والتراك (Radio)، والمهارات (Checkboxes)
3. **المراجعة:** عرض كل البيانات + زرار Submit

- Progress bar بيوضح إنت في أنهي خطوة
- **Validation** لكل خطوة قبل ما تروح للي بعدها، والأخطاء تظهر تحت كل input
- تقدر ترجع لخطوة قبلها والبيانات **متضيعش**
- State واحد للفورم كله (object)، وبتحدّثه **immutably**
- بعد الـ Submit: رسالة نجاح والفورم يتصفّر

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

احفظ الفورم في Local Storage أثناء ما المستخدم بيكتب، فلو قفل الصفحة بالغلط يلاقي بياناته لما يرجع.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف ليه `count = count + 1` مش بتغيّر حاجة في الصفحة
- [ ] أعرف ليه `state.push(item)` غلط، وإيه الصح
- [ ] أعرف إن تحديث الـ State مش بيحصل في نفس اللحظة (batching)
- [ ] أعرف إمتى أستخدم الـ updater function `prev => ...`
- [ ] أعرف الفرق بين Controlled و Uncontrolled input

</details>

### أخطاء شائعة

- **State لحاجة ممكن تتحسب.** لو عندك `items` و `total`، الـ `total` مش state، احسبه من `items`.
- **إنك تغيّر الـ object جوا الـ state مباشرة** (`user.name = "x"`). لازم object جديد: `{ ...user, name: "x" }`.
- **`onClick={handleClick()}`** بدل `onClick={handleClick}`. الأولى بتنفذ الـ function فورًا.

> **نصيحة منتور:** قبل ما تعمل `useState`، اسأل نفسك: "هل ده بيتغير؟ وهل ممكن أحسبه من حاجة موجودة؟" نص الـ state اللي المبتدئين بيعملوه مش محتاجينه.

---

<a id="week-21"></a>

## الأسبوع 21: Context و useEffect و Data Fetching

**الهدف:** تشارك داتا بين components بعيدة عن بعض، وتجيب داتا من API.

### المواضيع

- Communication بين الـ components: Props و Lifting State Up
- **Prop Drilling** والمشكلة بتاعته
- **`useContext`**
- **`useEffect`**: إمتى بيشتغل، والـ Dependencies، والـ **Cleanup**
- **API Requests** في React
- Loading و Error States
- i18n وتغيير اتجاه الصفحة (RTL / LTR)

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [ترميز: الدروس من 44 لـ 51 (Props و Context)](https://www.youtube.com/watch?v=nalt9TkgOlE&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=48) | 1.5 ساعة |
| الأساسي | [ترميز: الدروس من 97 لـ 109 (API و useEffect و مشروع الطقس)](https://www.youtube.com/watch?v=EJ7-xQ1l5-c&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=102) | 2.5 ساعة |
| مرجع | [Synchronizing with Effects - react.dev](https://react.dev/learn/synchronizing-with-effects) | |
| مرجع | [You Might Not Need an Effect - react.dev](https://react.dev/learn/you-might-not-need-an-effect) | **اقراها**، وهتوفر عليك bugs كتير |

### التاسك: Movies App (نسخة React)

لو عملت Movies Explorer في مشروع المستوى التاني، اعمله تاني بـ React. ولو عملت حاجة تانية، اعمله دلوقتي باستخدام [TMDB API](https://www.themoviedb.org/documentation/api) أو [DummyJSON](https://dummyjson.com/):

- لستة أفلام أو منتجات من الـ API، وبحث بـ debounce
- **Custom Hook** اسمه `useFetch<T>(url)` بيرجع `{ data, isLoading, error }`
- **ThemeContext** للـ Dark Mode
- **FavoritesContext** للمفضلة (بتتحفظ في Local Storage)
- الـ Cleanup صح: لو المستخدم كتب بسرعة، متعرضش نتيجة request قديم (`AbortController`)

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

اعمل اللغة عربي و إنجليزي بزرار، والصفحة تقلب RTL و LTR (زي ما اتعمل في مشروع الطقس في كورس ترميز).

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين `useEffect(fn)`، و `useEffect(fn, [])`، و `useEffect(fn, [x])`
- [ ] أعرف إمتى الـ cleanup function بتشتغل، وليه مهمة
- [ ] أعرف ليه الـ Effect بيشتغل مرتين في Development (Strict Mode)
- [ ] أعرف إمتى أستخدم Context، وإمتى props عادية أحسن
- [ ] أقدر أكتب Custom Hook

</details>

### أخطاء شائعة

- **`useEffect` عشان تحسب حاجة من الـ state.** ده مش محتاج effect، احسبها وقت الـ render.
- **Infinite loop:** effect بيعمل `setState` وفي نفس الوقت الـ state ده في الـ dependencies.
- **Context لكل حاجة.** Context مش State Management، هو طريقة **توصيل** بس. وأي تغيير فيه بيعمل re-render لكل اللي بيستخدمه.

> **نصيحة منتور:** `useEffect` هو أكتر hook بيتستخدم غلط في React. القاعدة: **Effect = مزامنة مع حاجة برا React** (API، و timer، و DOM، و Local Storage). لو مفيش حاجة برا React، غالبًا مش محتاج effect.

---

<a id="week-22"></a>

## الأسبوع 22: React Router

**الهدف:** تعمل أبلكيشن فيه صفحات كتير من غير ما الصفحة تعمل reload.

### المواضيع

- يعني إيه SPA، والفرق بين CSR و SSR
- تسطيب React Router
- Routes و `Link` و `NavLink`
- **Dynamic Routes** و `useParams`
- صفحة 404
- **Nested Routes** و Layouts و `Outlet`
- `useNavigate` و `useSearchParams`
- Protected Routes

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [ترميز: الدروس من 52 لـ 58](https://www.youtube.com/watch?v=bkj8obp1XmA&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=55) | 1.5 ساعة |
| مرجع | [React Router Docs](https://reactrouter.com/home) | |
| مرجع | [React Router: Declarative Mode Installation](https://reactrouter.com/start/declarative/installation) | |

> React Router v7 فيه 3 modes. استخدم **Declarative Mode**، لأنه الأقرب للي في الكورس والأبسط للبداية.

### التاسك: أبلكيشن متعدد الصفحات

كمّل على Movies App (أو اعمل مشروع جديد) وضيف:

- `/`: الرئيسية
- `/movies`: اللستة، والبحث والفلتر **في الـ URL** (`?q=batman&genre=action`) بـ `useSearchParams`
- `/movies/:id`: صفحة التفاصيل
- `/favorites`: المفضلة
- `/login`: صفحة login وهمية (بتحط user في Context)
- `/profile`: **Protected**، ولو مش عامل login يرجعك لـ `/login`
- صفحة 404 محترمة
- Layout مشترك فيه Navbar و Footer، و `NavLink` بيوضح إنت في أنهي صفحة

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

> **مهم في الـ Deploy:** لو عملت refresh على `/movies/5` على Netlify أو Vercel وطلعلك 404، دوّر على "SPA redirect rules" للمنصة اللي بتستخدمها.

### تحدي إضافي

**Lazy Loading** للصفحات: كل صفحة تتحمّل لما تروحلها بس (`React.lazy` + `Suspense`).

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين `<a>` و `<Link>`
- [ ] أعرف الفرق بين `useParams` و `useSearchParams`
- [ ] أعرف ليه ممكن أحط الـ state في الـ URL بدل `useState`
- [ ] أقدر أعمل Protected Route
- [ ] أعرف ليه الـ refresh بيدّي 404 على السيرفر في الـ SPA وإزاي أحلها

</details>

### أخطاء شائعة

- **`<a href>` بدل `<Link>`.** الصفحة هتعمل reload كامل وكل الـ state هتضيع.
- **إنك تنسى `<Outlet />`** في الـ layout، والصفحات الداخلية متظهرش.

> **نصيحة منتور:** الـ URL هو أقدم وأحسن State Management في الويب. أي حاجة المستخدم ممكن يحب يبعتها لحد (بحث، أو فلتر، أو صفحة)، حطها في الـ URL.

---

<a id="week-23"></a>

## الأسبوع 23: Styling و Component Libraries

**الهدف:** تعرف الطرق المختلفة لعمل styles في React، وتستخدم component library بذكاء.

### المواضيع

- طرق الـ Styling: CSS عادي، و CSS Modules، و **Tailwind**
- Tailwind مع React: الـ classes الـ conditional (`clsx`)
- **Component Libraries:** يعني إيه، وإمتى تستخدمها
- **shadcn/ui** (الأكثر استخدامًا حاليًا مع Tailwind)
- Material UI (MUI): Theme، و Icons، و Layout
- Icons (`lucide-react`)

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [ترميز: الدروس من 59 لـ 64 (Material UI)](https://www.youtube.com/watch?v=qwtcYDWf1EU&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=62) | 57 دقيقة |
| الأساسي | [Triangles: Landing Page بـ React 19 + Tailwind 4 ونشرها على Vercel](https://www.youtube.com/watch?v=T9iM1LVNKec&list=PLdnrjoDUmGZ8Q9Dq9ebR9v1xEgqJ6tcfx&index=11) | ساعة |
| الأساسي | [shadcn/ui Docs](https://ui.shadcn.com/docs) | إنجليزي، اقرا Introduction و Installation (Vite) |
| تطبيق | [ترميز: مشروع قائمة المهام (الدروس 65 لـ 84)](https://www.youtube.com/watch?v=nRsXnEIyPog&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=68) | 4 ساعات، **اختياري** |

### التاسك: UI Kit صغير

اعمل صفحة "**Component Gallery**" فيها components إنت عاملها بـ **Tailwind** + **shadcn/ui**:

- `Button` (variants و sizes و loading state)
- `Input` مع label و error message
- `Card`
- `Modal` أو `Dialog`
- `Toast` (رسالة بتظهر وتختفي)
- `Tabs`
- `Dropdown Menu`
- كله بيدعم **Dark Mode**

وبعدين استخدمهم في Movies App بدل الـ styles القديمة.

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

اعمل `Toast` system كامل بـ Context: `const { toast } = useToast()` من أي component، و `toast.success("تم الحفظ")`.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين component library زي MUI، و shadcn/ui اللي بينسخ الكود عندك
- [ ] أعرف إزاي أعمل class شرطي في Tailwind بشكل نضيف
- [ ] أعرف إمتى أستخدم library وإمتى أعمل الـ component بنفسي
- [ ] الـ components بتاعتي شغالة بالكيبورد (Tab و Enter و Escape)

</details>

### أخطاء شائعة

- **إنك تسطب 3 component libraries في نفس المشروع.** اختار واحدة.
- **إنك تستخدم library ومتعرفش تعدّل فيها.** لو مش عارف تغيّر لون الزرار، يبقى إنت مش متحكم في المشروع.

> **نصيحة منتور:** في الشغل الحقيقي نادرًا ما هتبني Modal أو Dropdown من الصفر، لأن الـ accessibility بتاعتهم صعبة جدًا. بس لازم تكون **بنيت واحد مرة** عشان تفهم الـ library بتعمل إيه.

---

<a id="week-24"></a>

## الأسبوع 24: State Management

**الهدف:** تدير State معقدة ومشتركة في أبلكيشن كبير.

### المواضيع

- إمتى `useState` و Context مش كفاية
- **`useReducer`**: Actions و Reducer، و Reducer + Context
- **Redux Toolkit:** Store، و Slices، و `useSelector`، و `useDispatch`، و Async Thunks، و DevTools
- **Zustand:** البديل الأخف والأبسط
- Client State vs Server State (مقدمة للأسبوع الجاي)

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [ترميز: useReducer (الدروس من 91 لـ 94)](https://www.youtube.com/watch?v=_IOM9XtJAvE&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=95) | ساعتين |
| الأساسي | [Simple Arab Code: Redux Toolkit من 1 لـ 13](https://www.youtube.com/watch?v=G3jSV8p9li0&list=PLxRKoQzM5m3J6gDMz-_eqLvxIR6UH0Pf7&index=1) | 2.5 ساعة |
| البديل | [ترميز: Redux (الدروس من 110 لـ 124)](https://www.youtube.com/watch?v=7bPnRc_BDe8&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=115) | 3.5 ساعة |
| الأساسي | [Zustand: Introduction](https://zustand.docs.pmnd.rs/learn/getting-started/introduction) | إنجليزي، قصير جدًا |
| مرجع | [Scaling Up with Reducer and Context - react.dev](https://react.dev/learn/scaling-up-with-reducer-and-context) | |
| مرجع | [Redux Toolkit Quick Start](https://redux-toolkit.js.org/tutorials/quick-start) | |

### التاسك: Shopping Cart

اعمل متجر صغير بـ [DummyJSON Products](https://dummyjson.com/):

- صفحة منتجات، وصفحة منتج، وصفحة Cart
- **Cart بـ Redux Toolkit:** إضافة، وحذف، وتغيير الكمية، والإجمالي، والخصم بكوبون
- **UI State بـ Zustand:** Sidebar مفتوح ولا مقفول، و Theme
- الـ Cart بيتحفظ في Local Storage
- أيقونة الـ Cart في الـ Navbar فيها عدد المنتجات

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

اعمل نفس الـ Cart بـ Zustand بس، وقارن: كام سطر في كل نسخة؟ وأنهي أسهل في القراية؟ اكتب رأيك في الـ README.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف إمتى أحتاج State Management library، وإمتى مش محتاجها
- [ ] أعرف الفرق بين `useState` و `useReducer`، وإمتى أستخدم كل واحد
- [ ] أفهم الـ Redux flow: Action، و Reducer، و Store، و UI
- [ ] أعرف ليه Redux Toolkit بيسمحلي أكتب `state.items.push()` (Immer)
- [ ] أعرف الفرق بين Redux و Zustand

</details>

### أخطاء شائعة

- **كل حاجة في Redux.** الـ state بتاعة input في فورم مكانها `useState`، مش الـ global store.
- **داتا الـ API في Redux.** دي **Server State**، ومكانها الأسبوع الجاي.

> **نصيحة منتور:** Redux Toolkit لسه موجود في مشاريع وشركات كتير جدًا في مصر، فلازم تعرفه. بس في المشاريع الجديدة، Zustand + TanStack Query بيغطّوا أغلب الاحتياجات بكود أقل بكتير.

---

<a id="week-25"></a>

## الأسبوع 25: TanStack Query

**الهدف:** تتعامل مع داتا السيرفر بالطريقة الاحترافية: Caching، و Refetching، و Mutations.

### المواضيع

- Server State vs Client State
- ليه `useEffect` + `fetch` مش كفاية في المشاريع الكبيرة
- `useQuery`: Query Keys، و `staleTime`، و Caching
- DevTools
- Dependent و Enabled Queries
- Pagination
- Prefetching
- **`useMutation`** و Invalidate Queries
- Optimistic Updates

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [kimz codes: TanStack Query بالعربي من 1 لـ 19](https://www.youtube.com/watch?v=KIS-MJfuPDY&list=PLejc1JbD4ZFRubkv6hV2D3r3eDoXTGHcF&index=1) | ساعتين |
| تكملة | [kimz codes: Optimistic Updates من 20 لـ 22](https://www.youtube.com/watch?v=9M6A2tfis-g&list=PLejc1JbD4ZFRubkv6hV2D3r3eDoXTGHcF&index=20) | 28 دقيقة |
| مرجع | [TanStack Query: Overview](https://tanstack.com/query/latest/docs/framework/react/overview) | |

### التاسك: Dashboard بـ Server State

اعمل Admin Dashboard لإدارة منتجات أو Posts باستخدام [DummyJSON](https://dummyjson.com/):

- جدول فيه البيانات مع **Pagination** و بحث
- صفحة تفاصيل لكل عنصر
- **Add و Edit و Delete** بـ `useMutation`
- بعد أي تعديل، الجدول يتحدث (`invalidateQueries`)
- Skeleton Loading بدل الـ spinner
- **مفيش ولا `useEffect` لجلب داتا** في المشروع كله

> **ملاحظة:** DummyJSON بيعمل simulation للـ add و edit و delete بس مش بيحفظهم فعلًا. ده كويس للتدريب، وهتشوف التغيير في الـ response.

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

**Optimistic Delete:** العنصر يختفي من الجدول فورًا، ولو الـ request فشل يرجع تاني مع رسالة خطأ.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين Server State و Client State
- [ ] أعرف يعني إيه `staleTime`، والفرق بينه وبين `gcTime`
- [ ] أعرف ليه الـ Query Key لازم يحتوي على كل المتغيرات (`['products', page, search]`)
- [ ] أقدر أعمل mutation وأحدّث الداتا بعدها
- [ ] بستخدم React Query DevTools وفاهم بيوريني إيه

</details>

### أخطاء شائعة

- **Query Key ثابت** (`['products']`) والصفحة بتتغير. الداتا مش هتتحدث.
- **إنك تنسخ داتا الـ query في `useState`.** استخدمها مباشرة من `useQuery`.

> **نصيحة منتور:** بعد ما تجرب TanStack Query، مش هترجع لـ `useEffect` + `fetch` تاني. ودي حاجة بتبان جدًا في الـ code review.

---

<a id="week-26"></a>

## الأسبوع 26: Testing

**الهدف:** تكتب tests بتتأكد إن الكود شغال، وتمسك أي حاجة تبوظ لما تعدّل بعدين.

### المواضيع

- ليه نكتب Tests، وأنواعها: Unit، و Integration، و E2E
- **Vitest:** `describe`، و `it`، و `expect`، و Matchers
- **React Testing Library:** `render`، و `screen`، و Queries (`getByRole`، و `getByText`، ...)
- User Events
- Async Tests
- Mocking (functions و API calls)
- TDD (مقدمة)

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Index Academy: React Testing بالعربي من 01 لـ 15](https://www.youtube.com/watch?v=hDZjJPPsWJw&list=PLDQ11FgmbqQOFLSRv-Ya39CchDjP1BLju&index=2) | 2.5 ساعة |
| مرجع | [Vitest: Getting Started](https://vitest.dev/guide/) | |
| مرجع | [React Testing Library: Intro](https://testing-library.com/docs/react-testing-library/intro/) | |
| مرجع | [Playwright: Installation](https://playwright.dev/docs/intro) | للتحدي الإضافي |

> **عن Jest و Vitest:** الكورس العربي بيستخدم **Jest**. إحنا هنستخدم **Vitest** لأنه شغال مع Vite من غير أي ظبط. الكتابة **تقريبًا نفسها بالظبط** (`describe`، و `it`، و `expect`)، والفرق إنك هتكتب `vi.fn()` بدل `jest.fn()`. فاتفرج على الكورس، واكتب بـ Vitest.

### التاسك: Tests للـ Cart

ارجع لمشروع الـ Shopping Cart (الأسبوع 24) واكتب:

- **Unit tests** للـ reducer أو الـ slice: إضافة، وحذف، وتغيير الكمية، والإجمالي، والكوبون (5 tests على الأقل)
- **Unit tests** لأي utility functions (تنسيق السعر مثلًا)
- **Component tests** بـ React Testing Library:
  - `ProductCard`: بيعرض الاسم والسعر، والضغط على "Add to Cart" بيستدعي الـ function
  - `CartPage`: بيعرض "Cart فاضي" لو مفيش حاجة، وبيعرض الإجمالي صح
- **Mock** للـ API في test واحد على الأقل
- `npm run test` كله أخضر

**التسليم:** على الداشبورد: لينك الـ Repo + Screenshot لنتيجة الـ tests.

### تحدي إضافي

اكتب **E2E test واحد** بـ Playwright: يفتح الموقع، ويضيف منتج للـ Cart، ويروح لصفحة الـ Cart، ويتأكد إن المنتج موجود.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين Unit و Integration و E2E
- [ ] أعرف ليه `getByRole` أحسن من `getByTestId` في أغلب الحالات
- [ ] أعرف الفرق بين `getBy`، و `queryBy`، و `findBy`
- [ ] أقدر أعمل mock لـ function وأتأكد إنها اتنادت
- [ ] بكتب tests بتختبر **اللي المستخدم بيشوفه**، مش تفاصيل الكود

</details>

### أخطاء شائعة

- **إنك تختبر الـ implementation** (اسم state، أو عدد re-renders). اختبر اللي المستخدم بيشوفه ويعمله.
- **Tests بتعدّي دايمًا.** جرّب تبوّظ الكود وشوف الـ test بيفشل ولا لأ. لو مش بيفشل، يبقى مش بيختبر حاجة.

> **نصيحة منتور:** مش لازم 100% coverage. ابدأ بـ test للحاجات اللي **لو باظت هتعمل مشكلة كبيرة**: الحسابات، والـ cart، والـ auth.

---

<a id="week-27"></a>

## الأسبوع 27: Performance و Accessibility

**الهدف:** تخلي الأبلكيشن سريع، وكل الناس تقدر تستخدمه.

### المواضيع

**Performance:**
- إزاي React بيعمل re-render، وإمتى ده يبقى مشكلة
- React DevTools Profiler
- `memo` و `useMemo` و `useCallback`، و**إمتى مش محتاجهم**
- **React Compiler**: بيعمل الـ memoization لوحده
- Code Splitting و `lazy`
- Core Web Vitals: LCP، و INP، و CLS
- Lighthouse
- الصور: `loading="lazy"`، و الأحجام، و WebP و AVIF
- حجم الـ Bundle

**Accessibility:**
- ليه الـ a11y مهمة
- Semantic HTML في React
- الكيبورد و Focus Management
- ARIA (وإمتى **متستخدموش**)
- Color Contrast
- Screen Readers

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [ترميز: Caching The Computations Using useMemo (الدرس 86)](https://www.youtube.com/watch?v=5xWJIRJDQXM&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=89) | 16 دقيقة |
| الأساسي | [Ahmed Saber: Web Accessibility 101](https://www.youtube.com/playlist?list=PLNknCqb-phEjLVnCbtVTJnWYml0zRvt5Y) | 2.5 ساعة |
| الأساسي | [Learn Performance - web.dev](https://web.dev/learn/performance) | إنجليزي، اختار الأجزاء اللي محتاجها |
| مرجع | [memo](https://react.dev/reference/react/memo) · [useMemo](https://react.dev/reference/react/useMemo) · [lazy](https://react.dev/reference/react/lazy) - react.dev | |
| مرجع | [React Compiler - react.dev](https://react.dev/learn/react-compiler) | |
| مرجع | [Web Vitals - web.dev](https://web.dev/articles/vitals) | |
| مرجع | [Learn Accessibility - web.dev](https://web.dev/learn/accessibility) | |
| أداة | [Lighthouse](https://developer.chrome.com/docs/lighthouse/overview) · [WAVE](https://wave.webaim.org/) | |

### التاسك: Audit وتحسين مشروع

اختار أكبر مشروع عملته في المستوى ده (غالبًا الـ Dashboard أو الـ Cart):

1. شغّل **Lighthouse** (Mobile) وخد Screenshot **قبل**
2. شغّل **React DevTools Profiler** ودوّر على re-renders ملهاش لازمة
3. اعمل **Code Splitting** للصفحات
4. حسّن الصور
5. **a11y:** جرّب الأبلكيشن بالكيبورد بس، وصلّح أي حاجة مش شغالة. شغّل WAVE وصلّح الأخطاء
6. خد Screenshot **بعد**
7. اكتب في الـ README جدول: **المشكلة، و عملت إيه، و النتيجة قبل وبعد**

**التسليم:** على الداشبورد: لينك الـ Repo (فيه الـ README بالجدول) + Screenshots قبل وبعد.

### تحدي إضافي

شغّل الأبلكيشن بـ **Screen Reader** (NVDA على Windows، أو VoiceOver على Mac، أو TalkBack على Android) وحاول تستخدمه وعينك مقفولة لمدة 5 دقايق. اكتب إيه اللي حسيت بيه.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف إيه اللي بيعمل re-render لـ component في React
- [ ] أعرف إمتى `useMemo` و `useCallback` بيفيدوا، وإمتى بيضرّوا
- [ ] أعرف يعني إيه LCP و INP و CLS
- [ ] أقدر أقرا تقرير Lighthouse وأعرف أبدأ منين
- [ ] الأبلكيشن بتاعي شغال بالكيبورد كله
- [ ] أعرف إن "**No ARIA is better than bad ARIA**"

</details>

### أخطاء شائعة

- **`useMemo` على كل حاجة.** الـ memoization ليها تكلفة. استخدمها لما تقيس وتلاقي مشكلة فعلًا.
- **`<div onClick>` بدل `<button>`.** مش هيشتغل بالكيبورد، والـ Screen Reader مش هيعرف إنه زرار.

> **نصيحة منتور:** **قيس قبل ما تحسّن.** أغلب مشاكل الـ performance اللي بتشوفها في مشاريع المبتدئين جاية من صور كبيرة وحاجات بتتحمّل مش محتاجينها، مش من re-renders.

---

<a id="week-28"></a>

## الأسبوع 28: Next.js، الأساسيات والـ Routing

**الهدف:** تفهم Next.js بيضيف إيه على React، وتبني صفحات بالـ App Router.

### المواضيع

- يعني إيه Meta-framework، وليه Next.js
- CSR vs SSR vs SSG
- إنشاء مشروع وفهم هيكل الملفات
- **App Router:** الـ routing بالفولدرات
- `Link` والتنقل
- Dynamic Routes و Nested Routes
- **Layouts** و Nested Layouts
- Params في الـ dynamic routes

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [سعد السطوف: كورس Next.js كامل 2026 من 1 لـ 12](https://www.youtube.com/watch?v=P6n44p4k9U8&list=PLSDhifuM5C420tyw98jx-ZesncZVtOyPB&index=1) | 1.5 ساعة |
| الأساسي | [Learn Next.js](https://nextjs.org/learn) | الكورس الرسمي، إنجليزي، تفاعلي ومجاني |
| مرجع | [Next.js Docs](https://nextjs.org/docs) | |

### التاسك: Blog بـ Next.js

ابدأ مشروع Blog (هتكمله الأسبوع الجاي):

- `/`: الرئيسية، فيها آخر البوستات
- `/blog`: كل البوستات
- `/blog/[slug]`: صفحة البوست
- `/about`
- Layout رئيسي فيه Navbar و Footer، و Layout مختلف لصفحات الـ blog فيه sidebar
- البوستات حاليًا في ملف `data.ts` (array of objects)
- TypeScript و Tailwind

**التسليم:** على الداشبورد: لينك الـ Repo.

### تحدي إضافي

اكتب البوستات كملفات **Markdown** واعرضها (دوّر على MDX في Next.js docs).

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين CSR و SSR و SSG، وإمتى كل واحد مناسب
- [ ] أعرف إزاي الفولدرات بتتحول لـ routes في الـ App Router
- [ ] أعرف `page.tsx` و `layout.tsx` الفرق بينهم إيه
- [ ] أقدر أعمل dynamic route وآخد الـ params

</details>

### أخطاء شائعة

- **إنك تتفرج على كورس بيستخدم الـ Pages Router (`pages/`).** إحنا بنستخدم **App Router (`app/`)**، وده الحالي والـ default.
- **إنك تحط `"use client"` في أول كل ملف.** ده موضوع الأسبوع الجاي، بس باختصار: متعملش كده.

> **نصيحة منتور:** Next.js في الأول هيحسسك إنك بتتعلم React من جديد، بس ده مش حقيقي. كل اللي اتعلمته شغال زي ما هو، Next.js بس بيضيف **إنت بترندر فين** (Server ولا Client).

---

<a id="week-29"></a>

## الأسبوع 29: Next.js، Data و SEO و Deploy + الشغل مع الـ AI

**الهدف:** تكمّل الـ Blog بداتا حقيقية و SEO وترفعه، وتتعلم إزاي تستخدم الـ AI كأداة شغل حقيقية.

### المواضيع

**Next.js:**
- **Server Components vs Client Components** و `"use client"`
- Data Fetching في Server Components
- Route Handlers (API Routes)
- `loading.tsx` و `error.tsx` و `not-found.tsx`
- **Metadata و SEO**
- `next/image` و `next/font`
- Deploy على Vercel

**الشغل مع الـ AI:**
- إزاي تكتب prompt كويس لمهمة برمجية (السياق، والقيود، والمطلوب بالظبط)
- استخدامه في: الـ boilerplate، والـ tests، وشرح كود مش فاهمه، و code review
- **إزاي تراجع كود الـ AI:** متقبلش حاجة مش فاهمها، واختبر كل حاجة
- الحاجات اللي الـ AI بيغلط فيها كتير: APIs قديمة، و packages مش موجودة، وحلول أعقد من اللازم

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [سعد السطوف: كورس Next.js من 13 لـ 20](https://www.youtube.com/watch?v=cTNbmYbEa9w&list=PLSDhifuM5C420tyw98jx-ZesncZVtOyPB&index=13) | ساعة |
| تكملة | [سعد السطوف: المستوى التاني (Auth و Middleware و Deploy) من 21 لـ 30](https://www.youtube.com/watch?v=ZzDG94HAEgM&list=PLSDhifuM5C420tyw98jx-ZesncZVtOyPB&index=21) | ساعتين، **اختياري** |
| مرجع | [Learn Next.js](https://nextjs.org/learn) | كمّل الفصول اللي فاتتك |
| مرجع | [GitHub Copilot Docs](https://docs.github.com/en/copilot) | |

### التاسك: تكملة الـ Blog + Deploy

- البوستات تيجي من API (مثلًا [DummyJSON Posts](https://dummyjson.com/)) في **Server Component**
- زرار Like و Comment form يبقوا **Client Components** (وده المكان الوحيد اللي فيه `"use client"`)
- Route Handler واحد على الأقل (`/api/...`)
- `loading.tsx` بـ skeleton، و `error.tsx`، و `not-found.tsx`
- **Metadata** لكل صفحة، و dynamic metadata لصفحة البوست (العنوان والوصف من البوست نفسه)
- كل الصور بـ `next/image`، والخط بـ `next/font`
- **Deploy على Vercel**
- Lighthouse SEO و Performance **90+**

**مهمة الـ AI:**
استخدم أي أداة AI عشان:
1. تكتب tests لـ component واحد
2. تعمل review لملف من ملفاتك
3. تشرحلك حاجة في Next.js مكنتش فاهمها

واكتب في ملف `AI_LOG.md`: كتبت إيه بالظبط (الـ prompt)، وهو رد بإيه، و**إيه اللي كان غلط أو محتاج تعديل في رده**.

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live + ملف `AI_LOG.md`.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين Server Component و Client Component، وإمتى أحتاج `"use client"`
- [ ] أعرف ليه مينفعش أستخدم `useState` في Server Component
- [ ] أقدر أجيب داتا في Server Component من غير `useEffect`
- [ ] أعرف إزاي أعمل Metadata ديناميك
- [ ] رفعت مشروع Next.js على Vercel
- [ ] بقدر أراجع كود الـ AI وأمسك غلطه

</details>

### أخطاء شائعة

- **`"use client"` في الـ layout.** كده كل الأبلكيشن بقى Client، وضاعت فايدة Next.js.
- **إنك تطلب من الـ AI "اعملّي blog بـ Next.js".** هيطلعلك كود ممكن يكون بنسخة قديمة أو بالـ Pages Router. ادّيله سياق: النسخة، والـ App Router، والملف اللي إنت فيه، والمطلوب بالظبط.

> **نصيحة منتور:** الـ AI مش هياخد شغلك. **المبرمج اللي بيعرف يستخدم الـ AI كويس** هو اللي ممكن ياخده. والفرق إن الأول بيعرف يمسك أغلاطه، لأنه فاهم الأساسيات اللي إنت قضيت 28 أسبوع تتعلمها.

---

<a id="week-30"></a>

## الأسبوع 30: مشروع التخرج

**الهدف:** تبني أبلكيشن كامل يبقى **أقوى حاجة في الـ Portfolio بتاعك**.

### المشروع: اختار فكرة

| الفكرة | تفاصيل |
| :--- | :--- |
| **E-commerce** | منتجات، وفلاتر، وبحث، وCart، وCheckout (وهمي)، وصفحة طلبات |
| **Admin Dashboard** | Charts، وجداول بـ Pagination و Sort و Filter، و CRUD كامل، و Dark Mode |
| **Learning Platform** | كورسات، ودروس، وتقدّم المستخدم، وكويزات |
| **Job Board** | وظايف، وفلاتر، وصفحة شركة، وحفظ الوظايف، وتقديم |
| **Event Platform لـ CIS** | إيفنتات، وتسجيل، وتذاكر بـ QR Code، وصفحة للأدمن |
| **فكرتك إنت** | اتكلم مع المنتور الأول |

### المتطلبات

| المتطلب | التفاصيل |
| :--- | :--- |
| **التقنيات** | **Next.js** (App Router) أو **React + Vite**، و TypeScript (`strict`)، و Tailwind |
| **الصفحات** | 5 صفحات على الأقل، منهم dynamic routes |
| **State** | Zustand أو Redux Toolkit للـ Client State، و TanStack Query (أو Server Components في Next.js) للـ Server State |
| **Auth** | Login و Register (ممكن وهمي أو بـ API زي DummyJSON)، و Protected Routes |
| **Forms** | فورم واحد معقد على الأقل بـ validation |
| **Testing** | 10 tests على الأقل (Unit + Component) |
| **Performance** | Lighthouse **90+** في الأربع خانات |
| **Accessibility** | شغال بالكيبورد بالكامل |
| **Responsive** | Mobile First |
| **Git** | Branches و Pull Requests، و commits واضحة |
| **Deploy** | Live على Vercel |
| **README** | Screenshots أو GIF، ولينك Live، والتقنيات وليه اخترتها، وإزاي تشغّله، والتحديات اللي قابلتك، وإيه اللي هتضيفه لو عندك وقت |

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live + فيديو Demo (2-3 دقايق) بتشرح فيه المشروع.

<details>
<summary><b>Checklist آخر الرودماب</b></summary>

<br />

- [ ] أقدر أبني أبلكيشن React أو Next.js كامل من الصفر لوحدي
- [ ] بكتب TypeScript بشكل طبيعي
- [ ] بعرف أختار الأداة الصح للمشكلة (State، و Fetching، و Styling)
- [ ] بكتب tests للحاجات المهمة
- [ ] بفكر في الـ Performance والـ Accessibility من الأول، مش في الآخر
- [ ] GitHub بتاعي فيه 3 مشاريع كبيرة على الأقل Live، وبـ README محترم
- [ ] بستخدم الـ AI كأداة، وبعرف أمسك أغلاطه

</details>

> **نصيحة منتور:** مشروع واحد **كامل ومتعوب عليه** أحسن من 10 مشاريع tutorial. لما تقدّم على شغل، الـ interviewer هيفتح المشروع ده، وهيسألك "ليه عملت كده؟" في كل حتة. فخليك عارف إجابة كل سؤال.

---

## خلصت الرودماب. إيه بعد كده؟

**مبروك.** إنت عملت حاجة أغلب الناس اللي بيبدأوا بيبطّلوا في نصها.

الخطوات الجاية:

1. **Portfolio:** اعمل موقع شخصي بـ Next.js فيه مشاريعك
2. **Open Source:** دوّر على issues عليها `good first issue` في مشاريع بتستخدمها
3. **اتعلم Backend بسيط:** Node.js و Express، أو Route Handlers في Next.js مع Database، عشان تفهم الصورة كاملة
4. **قدّم على Internships** حتى لو حاسس إنك مش جاهز. إنت جاهز أكتر ما إنت فاكر.
5. **علّم غيرك:** اكتب بوست عن حاجة اتعلمتها، أو ساعد حد في المستوى الأول. **مفيش طريقة تتعلم بيها أحسن من إنك تشرح.**

**[الرجوع للخريطة](README.md)**

</div>
