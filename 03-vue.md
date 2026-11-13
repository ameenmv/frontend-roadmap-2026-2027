<div align="center">

<h1>المستوى التالت: Vue</h1>

<p><strong>Vue 3 · Vue Router · Pinia · TanStack Query · Testing · Performance · a11y · Nuxt</strong></p>

<p>
  <img src="https://img.shields.io/badge/Weeks-19_→_30-059669?style=for-the-badge" alt="Weeks 19-30" />
  <img src="https://img.shields.io/badge/Vue-3_Composition_API-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D" alt="Vue 3" />
  <img src="https://img.shields.io/badge/Nuxt-00DC82?style=for-the-badge&logo=nuxt&logoColor=white" alt="Nuxt" />
</p>

</div>

<div dir="rtl">

> **[الرجوع للخريطة](README.md)** · [المستوى الأول](01-beginner.md) · [المستوى التاني](02-intermediate.md) · [React](03-react.md) · Vue

---

## الحكاية

فاكر في الأسبوع 12 لما كنت بتحدّث الـ UI بإيدك كل ما الداتا تتغير؟ Vue بتقولك: **غيّر الداتا وبس، وأنا هحدّث الصفحة لوحدي.** ده اللي اسمه **Reactivity**، وهو قلب Vue.

Vue معروفة إنها **أسهل framework تبدأ بيه**: الـ template شبه HTML اللي إنت عارفه، والـ docs بتاعتها من أحسن الـ docs في الدنيا. وفي آخر المستوى هتتعلم **Nuxt** اللي بيحوّل Vue لـ framework كامل.

| الأسبوع | الموضوع | التاسك |
| :---: | :--- | :--- |
| 19 | [Template Syntax و Directives](#week-19) | تحويل Landing Page لـ Vue |
| 20 | [Composition API و Components](#week-20) | Multi-step Form |
| 21 | [Lifecycle و Watchers و Composables و Data Fetching](#week-21) | Movies App (نسخة Vue) |
| 22 | [Vue Router](#week-22) | أبلكيشن متعدد الصفحات |
| 23 | [Styling و Component Libraries](#week-23) | UI Kit صغير |
| 24 | [Pinia](#week-24) | Shopping Cart |
| 25 | [TanStack Query](#week-25) | Dashboard بـ Server State |
| 26 | [Testing](#week-26) | Tests للـ Cart |
| 27 | [Performance و Accessibility](#week-27) | Audit وتحسين مشروع |
| 28 | [Nuxt: الأساسيات والـ Routing](#week-28) | Blog بـ Nuxt |
| 29 | [Nuxt: Data و SEO و Deploy + الشغل مع الـ AI](#week-29) | تكملة الـ Blog + Deploy |
| 30 | [**مشروع التخرج**](#week-30) | أبلكيشن كامل |

> **قبل ما تبدأ:** المصدر العربي الأساسي في المستوى ده هو قناة **Vuejs Wisdom**: [Vue 3 Options API](https://www.youtube.com/playlist?list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV) و [Composition API](https://www.youtube.com/playlist?list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC) و [Nuxt 3](https://www.youtube.com/playlist?list=PLzjSlWqF2aTcdEs97QvAU13E07llvv3UO). والمرجع الرسمي **[vuejs.org](https://vuejs.org/guide/introduction.html)**، ودي من أحسن الـ docs اللي ممكن تقراها في حياتك، فاقراها.

> **Options API ولا Composition API؟** Vue فيها طريقتين تكتب بيهم. إحنا هنستخدم **Composition API** مع `<script setup>` لأنها الحالية والمستخدمة في المشاريع الجديدة وبتشتغل أحسن مع TypeScript. هنتفرج على أول جزء من كورس Options عشان الـ template والـ directives (وهي **نفسها بالظبط** في الطريقتين)، وبعدين نكمّل Composition.

> **عن TypeScript:** من النهارده، **كل مشروع Vue هتعمله بـ TypeScript** (`<script setup lang="ts">`). الكورسات أغلبها بـ JS، فدي فرصتك تتدرب. ولما تقف، افتح [Using Vue with TypeScript](https://vuejs.org/guide/typescript/overview.html).

---

<a id="week-19"></a>

## الأسبوع 19: Template Syntax و Directives

**الهدف:** تفهم إزاي Vue بتربط الداتا بالـ HTML، وتستخدم الـ directives الأساسية.

### المواضيع

- يعني إيه Vue، وليه
- إنشاء مشروع: `npm create vue@latest` (اختار TypeScript و Router و Pinia و Vitest و ESLint)
- **Template Syntax:** `{{ }}` و `v-bind` (`:`)
- **Events:** `v-on` (`@`) و Event Modifiers و Keyboard Modifiers
- **`v-model`** (Two-way Binding)
- Computed Properties
- Dynamic Classes و Styles
- **`v-if` و `v-show`**
- **`v-for`** و `:key`

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Vuejs Wisdom: Vue 3 من 1 لـ 15](https://www.youtube.com/watch?v=Vne-X1taBfI&list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV&index=1) | ساعتين |
| الأساسي | [Vue Tutorial (تفاعلي)](https://vuejs.org/tutorial/) | إنجليزي. **اختار Composition API و SFC من الإعدادات فوق** |
| مرجع | [Template Syntax - vuejs.org](https://vuejs.org/guide/essentials/template-syntax.html) | |

> الكورس بيكتب الـ JS بـ Options API (`data()`، و `methods`). ركّز على **الـ template** (اللي جوا `<template>`)، لأن ده اللي هيفضل زي ما هو. الجزء اللي جوا `<script>` هتكتبه بـ Composition من الأسبوع الجاي، والـ Tutorial الرسمي هيوريك الطريقة دي من دلوقتي.

### التاسك: تحويل Landing Page لـ Vue

خد مشروع الـ Landing Page بتاع الأسبوع 8، وحوّله لمشروع Vue:

- كل الحاجات المتكررة (كروت، و testimonials، ولينكات الـ navbar) تبقى **array of objects** في الـ script وتترسم بـ `v-for`
- قائمة الموبايل تفتح وتقفل بـ `v-if` أو `v-show` وزرار
- Pricing فيه Toggle بين **شهري وسنوي** والأسعار تتغير (computed)
- فورم "اشترك في النشرة" بـ `v-model` و validation بسيط
- لسه **component واحد** الأسبوع ده (هنقسّم الأسبوع الجاي)

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

خلّص الـ Vue Tutorial الرسمي كله (15 خطوة).

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين `v-if` و `v-show`، وإمتى أستخدم كل واحد
- [ ] أعرف ليه `:key` مهم مع `v-for`
- [ ] أعرف الفرق بين computed و method
- [ ] أعرف `v-model` بيعمل إيه من ورا الستارة (`:value` + `@input`)
- [ ] أعرف الـ shorthands: `:` لـ `v-bind` و `@` لـ `v-on`

</details>

### أخطاء شائعة

- **`v-if` و `v-for` على نفس العنصر.** استخدم `<template v-for>` أو computed بتعمل filter.
- **إنك تستخدم Vue CLI.** لو الكورس بيستخدم `vue create` (Vue CLI)، **استخدم `npm create vue@latest` بدلها**. Vue CLI مبقاش بيتطور، والمشاريع الجديدة كلها Vite.

> **نصيحة منتور:** docs بتاعة Vue مكتوبة كأنها كورس. لو عندك وقت، اقرا الـ **Essentials** كلها بالترتيب. هتلاقي إجابة أي سؤال عندك فيها.

---

<a id="week-20"></a>

## الأسبوع 20: Composition API و Components

**الهدف:** تكتب Vue بالطريقة الحديثة، وتقسم الأبلكيشن components بتتكلم مع بعض.

### المواضيع

- `<script setup>`
- **Reactivity:** `ref` و `reactive` (والفرق بينهم)
- Functions و `computed`
- Template Refs
- **Components** و Single File Components (`.vue`)
- **Props** (بـ TypeScript: `defineProps<{...}>()`)
- **Emits** (`defineEmits`)
- **Slots**
- Scoped Styles

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Vuejs Wisdom: Composition API من 1 لـ 6](https://www.youtube.com/watch?v=scY-dpK_Sl8&list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC&index=1)، و[8 (Emits)](https://www.youtube.com/watch?v=cTxEScjGvpU&list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC&index=8) | 57 دقيقة |
| الأساسي | [Vuejs Wisdom: Slots (درس 29 في كورس Options)](https://www.youtube.com/watch?v=kfFkZGYKZ3w&list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV&index=29) | 11 دقيقة |
| مرجع | [Reactivity Fundamentals - vuejs.org](https://vuejs.org/guide/essentials/reactivity-fundamentals.html) | |
| مرجع | [Props](https://vuejs.org/guide/components/props.html) · [Events](https://vuejs.org/guide/components/events.html) · [Slots](https://vuejs.org/guide/components/slots.html) | |

### التاسك: Multi-step Form

اعمل فورم تسجيل على 3 خطوات (زي فورم التقديم على كورس):

1. **البيانات الشخصية:** الاسم، والإيميل، والموبايل
2. **البيانات الأكاديمية:** الكلية، والسنة، والتراك (Radio)، والمهارات (Checkboxes)
3. **المراجعة:** عرض كل البيانات + زرار Submit

- كل خطوة **component منفصل**، والـ parent ماسك الداتا كلها
- الـ components بتاخد الداتا بـ **props** وبتبلّغ بالتغيير بـ **emits**
- `BaseInput` component بيستخدم `v-model` (`defineModel`) و يعرض الـ error
- `StepLayout` component فيه **slot** للمحتوى، و**named slot** للأزرار
- Progress bar و Validation لكل خطوة

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

احفظ الفورم في Local Storage أثناء ما المستخدم بيكتب (هتحتاج `watch`، فبص على الأسبوع الجاي).

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين `ref` و `reactive`، وليه الـ docs بتنصح بـ `ref`
- [ ] أعرف ليه محتاج `.value` في الـ script ومش محتاجه في الـ template
- [ ] أعرف إن الـ props **read-only**، والـ child بيبلّغ الـ parent بـ emit
- [ ] أعرف الفرق بين default slot و named slot
- [ ] أعرف `defineModel` بيعمل إيه

</details>

### أخطاء شائعة

- **إنك تعمل destructure لـ `reactive` object.** هيفقد الـ reactivity. استخدم `toRefs` أو `ref`.
- **إنك تعدّل prop جوا الـ child.** ابعت emit للـ parent وهو يعدّل.
- **إنك تنسى `.value`** في الـ script وتستغرب ليه الحاجة مش بتتغير.

> **نصيحة منتور:** قاعدة "**Props down, Events up**" هي أساس أي framework. الداتا بتنزل من الأب للابن، والأحداث بتطلع من الابن للأب. لو فهمتها كويس، هتفهم React و Angular و Svelte بنفس السهولة.

---

<a id="week-21"></a>

## الأسبوع 21: Lifecycle و Watchers و Composables و Data Fetching

**الهدف:** تجيب داتا من API، وتشارك داتا بين components بعيدة، وتعمل logic تقدر تستخدمه في أكتر من مكان.

### المواضيع

- **Lifecycle Hooks:** `onMounted` و `onUnmounted`
- **`watch` و `watchEffect`**
- **Provide / Inject**
- `v-model` على الـ components
- **API Requests** في Vue
- Loading و Error States
- **Composables:** الطريقة اللي Vue بتشارك بيها الـ logic (زي Custom Hooks في React)

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Vuejs Wisdom: Composition من 11 لـ 13 (Watch و Provide/Inject و Lifecycle)](https://www.youtube.com/watch?v=0GO4UunMALc&list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC&index=11) | 24 دقيقة |
| الأساسي | [Vuejs Wisdom: v-model و HTTP Requests (من 31 لـ 35 في كورس Options)](https://www.youtube.com/watch?v=0pODnNSy4oI&list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV&index=31) | 1.5 ساعة |
| الأساسي | [Composables - vuejs.org](https://vuejs.org/guide/reusability/composables.html) | **اقراها كلها**، فيها مثال `useFetch` |
| مرجع | [Lifecycle Hooks](https://vuejs.org/guide/essentials/lifecycle.html) · [Watchers](https://vuejs.org/guide/essentials/watchers.html) · [Provide / Inject](https://vuejs.org/guide/components/provide-inject.html) | |

### التاسك: Movies App (نسخة Vue)

لو عملت Movies Explorer في مشروع المستوى التاني، اعمله تاني بـ Vue. ولو عملت حاجة تانية، اعمله دلوقتي باستخدام [TMDB API](https://www.themoviedb.org/documentation/api) أو [DummyJSON](https://dummyjson.com/):

- لستة أفلام أو منتجات من الـ API، وبحث بـ debounce (`watch`)
- **Composable** اسمه `useFetch<T>(url)` بيرجع `{ data, isLoading, error }`، ولو الـ url كان `ref` يعيد الـ fetch لوحده لما يتغير
- `useTheme()` composable للـ Dark Mode
- المفضلة بـ **provide / inject** (وبتتحفظ في Local Storage)
- لو المستخدم كتب بسرعة، متعرضش نتيجة request قديم (`AbortController` + `onWatcherCleanup` أو الـ cleanup في `watch`)

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

اعمل `useLocalStorage<T>(key, defaultValue)` composable بيرجع `ref` بيتحفظ لوحده في Local Storage كل ما يتغير.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين `watch` و `watchEffect` و `computed`
- [ ] أعرف ليه الـ API call بيتعمل في `onMounted` أو في الـ setup نفسه
- [ ] أعرف إمتى أستخدم provide / inject، وإمتى props عادية أحسن
- [ ] أقدر أكتب Composable
- [ ] بنضّف أي timer أو listener في `onUnmounted`

</details>

### أخطاء شائعة

- **`watch` عشان تحسب قيمة من قيمة تانية.** ده شغل `computed`.
- **إنك تنسى تنضّف** `setInterval` أو event listener على `window`. هيفضل شغال حتى بعد ما الـ component يختفي.

> **نصيحة منتور:** الـ Composables هي أقوى حاجة في Vue 3. أي logic بتكتبه مرتين في component، اسأل نفسك: "ينفع يبقى composable؟"

---

<a id="week-22"></a>

## الأسبوع 22: Vue Router

**الهدف:** تعمل أبلكيشن فيه صفحات كتير من غير ما الصفحة تعمل reload.

### المواضيع

- يعني إيه SPA
- إنشاء Routes و `RouterLink` و `RouterView`
- Hash Mode vs History Mode
- Programmatic Navigation: `router.push` و `replace` و `go`
- **Dynamic Routes** و Params و Query
- **Nested Routes**
- صفحة 404
- **Navigation Guards** (`beforeEach`)
- `useRouter` و `useRoute` في Composition API

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Vuejs Wisdom: Vue Router من 40 لـ 54](https://www.youtube.com/watch?v=_Ppqm08EUfs&list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV&index=40) | ساعتين |
| الأساسي | [Vuejs Wisdom: Router و Route في Composition API](https://www.youtube.com/watch?v=snhWSqULz0Q&list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC&index=7) | 7 دقيقة |
| مرجع | [Vue Router Guide](https://router.vuejs.org/guide/) | |

### التاسك: أبلكيشن متعدد الصفحات

كمّل على Movies App (أو اعمل مشروع جديد) وضيف:

- `/`: الرئيسية
- `/movies`: اللستة، والبحث والفلتر **في الـ URL** (`?q=batman&genre=action`)
- `/movies/:id`: صفحة التفاصيل
- `/favorites`: المفضلة
- `/login`: صفحة login وهمية
- `/profile`: **Protected** بـ Navigation Guard، ولو مش عامل login يرجعك لـ `/login`
- صفحة 404 محترمة
- Layout مشترك فيه Navbar و Footer، والـ `RouterLink` الحالي واخد style مختلف (`router-link-active`)

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

> **مهم في الـ Deploy:** لو عملت refresh على `/movies/5` على Netlify أو Vercel وطلعلك 404، دوّر على "SPA redirect rules" للمنصة اللي بتستخدمها.

### تحدي إضافي

**Lazy Loading** للصفحات: `component: () => import('./views/MovieDetails.vue')`، وشوف في تاب Network إزاي كل صفحة بتتحمل لوحدها.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين `<a>` و `<RouterLink>`
- [ ] أعرف الفرق بين `useRouter` و `useRoute`
- [ ] أعرف الفرق بين params و query
- [ ] أقدر أعمل Navigation Guard
- [ ] أعرف الفرق بين Hash Mode و History Mode، وليه History محتاج ظبط على السيرفر

</details>

### أخطاء شائعة

- **إنك متعملش watch على الـ params.** لو روحت من `/movies/1` لـ `/movies/2`، الـ component **مش بيتعمل من الأول**، فالداتا مش هتتحدث لو جايبها في `onMounted` بس.

> **نصيحة منتور:** الـ URL هو أقدم وأحسن State Management في الويب. أي حاجة المستخدم ممكن يحب يبعتها لحد (بحث، أو فلتر، أو صفحة)، حطها في الـ URL.

---

<a id="week-23"></a>

## الأسبوع 23: Styling و Component Libraries

**الهدف:** تعرف الطرق المختلفة لعمل styles في Vue، وتستخدم component library بذكاء.

### المواضيع

- Scoped Styles و `lang` في `<style>`
- CSS Modules في Vue
- **Tailwind** مع Vue
- **Component Libraries:** يعني إيه، وإمتى تستخدمها
- **PrimeVue** و **shadcn-vue** و **Nuxt UI**
- Icons

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Vuejs Wisdom: Scoped و Lang](https://www.youtube.com/watch?v=FDUmao2ENkU&list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV&index=24) | 6 دقيقة |
| الأساسي | [Tailwind CSS: Installation with Vite](https://tailwindcss.com/docs/installation/using-vite) | نفس الخطوات اللي عملتها في الأسبوع 7 |
| الأساسي | [shadcn-vue](https://www.shadcn-vue.com/) أو [PrimeVue](https://primevue.org/) | اختار واحدة واقرا الـ Installation والـ Introduction |
| تطبيق | [Vuejs Wisdom: Todo App (Composition 15 و 16)](https://www.youtube.com/watch?v=QSBs0ceChnI&list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC&index=15) | 54 دقيقة، **اختياري** |

### التاسك: UI Kit صغير

اعمل صفحة "**Component Gallery**" فيها components إنت عاملها بـ **Tailwind** + library اخترتها:

- `BaseButton` (variants و sizes و loading state)
- `BaseInput` مع label و error message و `v-model`
- `BaseCard` بـ slots (header و default و footer)
- `BaseModal` (استخدم `<Teleport>`)
- `Toast` (رسالة بتظهر وتختفي)
- `Tabs`
- `Dropdown Menu`
- كله بيدعم **Dark Mode**

وبعدين استخدمهم في Movies App بدل الـ styles القديمة.

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

اعمل `useToast()` composable: `const toast = useToast()` من أي component، و `toast.success("تم الحفظ")`.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف `scoped` بيعمل إيه من ورا الستارة
- [ ] أعرف `<Teleport>` بيحل مشكلة إيه
- [ ] أعرف الفرق بين library زي PrimeVue، و shadcn-vue اللي بينسخ الكود عندك
- [ ] الـ components بتاعتي شغالة بالكيبورد (Tab و Enter و Escape)

</details>

### أخطاء شائعة

- **إنك تسطب أكتر من component library في نفس المشروع.** اختار واحدة.
- **إنك تستخدم library ومتعرفش تعدّل فيها.** لو مش عارف تغيّر لون الزرار، يبقى إنت مش متحكم في المشروع.

> **نصيحة منتور:** في الشغل الحقيقي نادرًا ما هتبني Modal أو Dropdown من الصفر، لأن الـ accessibility بتاعتهم صعبة جدًا. بس لازم تكون **بنيت واحد مرة** عشان تفهم الـ library بتعمل إيه.

---

<a id="week-24"></a>

## الأسبوع 24: Pinia

**الهدف:** تدير State مشتركة في أبلكيشن كبير بالأداة الرسمية لـ Vue.

### المواضيع

- إمتى props و provide / inject مش كفاية
- **Pinia:** يعني إيه Store
- `defineStore`: State، و Getters، و Actions
- **Setup Stores** (بنفس طريقة Composition API)
- `storeToRefs`
- Pinia DevTools
- Client State vs Server State (مقدمة للأسبوع الجاي)

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Algorithm Academy: Pinia من 1 لـ 7](https://www.youtube.com/watch?v=0e4D2ZJRe1E&list=PLfDx4cQoUNOZgZ5Lee5Lbj6jXlmCcupsm&index=1) | 50 دقيقة |
| الأساسي | [Pinia: Introduction](https://pinia.vuejs.org/introduction.html) | إنجليزي، قصير، و**شوف مثال الـ Setup Store** |
| مرجع | [Pinia: Core Concepts](https://pinia.vuejs.org/core-concepts/) | |

> الكورس بيكتب الـ stores بطريقة **Options Store** (`state`، و `getters`، و `actions`). جرّبها، وبعدين اكتب نفس الـ store بطريقة **Setup Store** (`ref`، و `computed`، و functions)، لأنها الأقرب لكل اللي اتعلمته.

### التاسك: Shopping Cart

اعمل متجر صغير بـ [DummyJSON Products](https://dummyjson.com/):

- صفحة منتجات، وصفحة منتج، وصفحة Cart
- **`useCartStore`:** إضافة، وحذف، وتغيير الكمية، والإجمالي (getter)، والخصم بكوبون
- **`useUiStore`:** Sidebar مفتوح ولا مقفول، و Theme
- الـ Cart بيتحفظ في Local Storage
- أيقونة الـ Cart في الـ Navbar فيها عدد المنتجات

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

اعمل Pinia Plugin بسيط بيحفظ أي store في Local Storage لوحده.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف إمتى أحتاج Pinia، وإمتى مش محتاجها
- [ ] أعرف الفرق بين Options Store و Setup Store
- [ ] أعرف ليه لازم `storeToRefs` لو هعمل destructure للـ state
- [ ] بستخدم Vue DevTools وأشوف الـ store بيتغير

</details>

### أخطاء شائعة

- **كل حاجة في Pinia.** الـ state بتاعة input في فورم مكانها `ref` في الـ component.
- **`const { count } = useStore()`** من غير `storeToRefs`، فالـ reactivity بتضيع.
- **داتا الـ API في Pinia.** دي **Server State**، ومكانها الأسبوع الجاي.

> **نصيحة منتور:** Pinia هي المكتبة الرسمية لـ Vue وبديلة Vuex. لو لقيت كورس أو مشروع بيستخدم Vuex، اعرف إنه قديم.

---

<a id="week-25"></a>

## الأسبوع 25: TanStack Query

**الهدف:** تتعامل مع داتا السيرفر بالطريقة الاحترافية: Caching، و Refetching، و Mutations.

### المواضيع

- Server State vs Client State
- ليه `onMounted` + `fetch` مش كفاية في المشاريع الكبيرة
- `useQuery`: Query Keys، و `staleTime`، و Caching
- DevTools
- Dependent و Enabled Queries
- Pagination
- **`useMutation`** و Invalidate Queries
- Optimistic Updates

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [TanStack Query: Vue Overview](https://tanstack.com/query/latest/docs/framework/vue/overview) | إنجليزي. اقرا Overview و Quick Start و Queries و Mutations و Query Invalidation |
| المفاهيم بالعربي | [kimz codes: TanStack Query بالعربي من 1 لـ 19](https://www.youtube.com/watch?v=KIS-MJfuPDY&list=PLejc1JbD4ZFRubkv6hV2D3r3eDoXTGHcF&index=1) | ساعتين |

> **ملاحظة:** مفيش كورس عربي لـ Vue Query تحديدًا. الكورس العربي ده بـ **React**، بس **المفاهيم هي هي بالظبط** (Query Keys، و staleTime، و Caching، و Mutations، و Invalidation)، والـ API شبه بعض جدًا (`useQuery({ queryKey, queryFn })`). اتفرج على المفاهيم، واكتب بـ Vue من الـ docs.

### التاسك: Dashboard بـ Server State

اعمل Admin Dashboard لإدارة منتجات أو Posts باستخدام [DummyJSON](https://dummyjson.com/):

- جدول فيه البيانات مع **Pagination** و بحث
- صفحة تفاصيل لكل عنصر
- **Add و Edit و Delete** بـ `useMutation`
- بعد أي تعديل، الجدول يتحدث (`invalidateQueries`)
- Skeleton Loading بدل الـ spinner
- **مفيش ولا `onMounted` لجلب داتا** في المشروع كله

> **ملاحظة:** DummyJSON بيعمل simulation للـ add و edit و delete بس مش بيحفظهم فعلًا. ده كويس للتدريب، وهتشوف التغيير في الـ response.

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live.

### تحدي إضافي

**Optimistic Delete:** العنصر يختفي من الجدول فورًا، ولو الـ request فشل يرجع تاني مع رسالة خطأ.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين Server State و Client State
- [ ] أعرف يعني إيه `staleTime`، والفرق بينه وبين `gcTime`
- [ ] أعرف إزاي أخلي الـ query تتحدث لوحدها لما `ref` يتغير (الـ query key يبقى reactive)
- [ ] أقدر أعمل mutation وأحدّث الداتا بعدها

</details>

### أخطاء شائعة

- **Query Key مش reactive.** لو `page` عبارة عن `ref`، حطه في الـ key كـ `ref` (أو getter) مش `.value`، عشان الـ query تتحدث لما يتغير.
- **إنك تنسخ داتا الـ query في `ref` تاني.** استخدمها مباشرة.

> **نصيحة منتور:** بعد ما تجرب TanStack Query، مش هترجع تكتب fetch في `onMounted` تاني. ودي حاجة بتبان جدًا في الـ code review.

---

<a id="week-26"></a>

## الأسبوع 26: Testing

**الهدف:** تكتب tests بتتأكد إن الكود شغال، وتمسك أي حاجة تبوظ لما تعدّل بعدين.

### المواضيع

- ليه نكتب Tests، وأنواعها: Unit، و Integration، و E2E
- **Vitest:** `describe`، و `it`، و `expect`، و Matchers
- **Vue Test Utils** و **Testing Library for Vue**: `mount` و `render`، و Queries
- اختبار Pinia stores
- Async Tests
- Mocking (functions و API calls)

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| المفاهيم بالعربي | [Index Academy: Testing بالعربي من 01 لـ 05](https://www.youtube.com/watch?v=hDZjJPPsWJw&list=PLDQ11FgmbqQOFLSRv-Ya39CchDjP1BLju&index=2) | 41 دقيقة |
| الأساسي | [Testing - vuejs.org](https://vuejs.org/guide/scaling-up/testing.html) | **ابدأ بيها**، بتشرح الصورة كلها |
| مرجع | [Vitest: Getting Started](https://vitest.dev/guide/) | |
| مرجع | [Vue Test Utils](https://test-utils.vuejs.org/guide/) · [Vue Testing Library](https://testing-library.com/docs/vue-testing-library/intro) | |
| مرجع | [Playwright: Installation](https://playwright.dev/docs/intro) | للتحدي الإضافي |

> **ملاحظة:** الفيديوهات العربي بـ React و Jest، بس أول 5 فيديوهات بيشرحوا **مفاهيم الـ testing** (ليه، وأنواعه، و Jest بيعمل إيه)، ودي نفسها في أي framework. Vitest بيتكتب **تقريبًا بنفس شكل Jest بالظبط**.

### التاسك: Tests للـ Cart

ارجع لمشروع الـ Shopping Cart (الأسبوع 24) واكتب:

- **Unit tests** للـ Cart Store: إضافة، وحذف، وتغيير الكمية، والإجمالي، والكوبون (5 tests على الأقل، استخدم `setActivePinia(createPinia())`)
- **Unit tests** لأي utility functions (تنسيق السعر مثلًا)
- **Component tests:**
  - `ProductCard`: بيعرض الاسم والسعر، والضغط على "Add to Cart" بيعمل emit أو بينادي الـ store
  - `CartPage`: بيعرض "Cart فاضي" لو مفيش حاجة، وبيعرض الإجمالي صح
- **Mock** للـ API في test واحد على الأقل
- `npm run test:unit` كله أخضر

**التسليم:** على الداشبورد: لينك الـ Repo + Screenshot لنتيجة الـ tests.

### تحدي إضافي

اكتب **E2E test واحد** بـ Playwright: يفتح الموقع، ويضيف منتج للـ Cart، ويروح لصفحة الـ Cart، ويتأكد إن المنتج موجود.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين Unit و Integration و E2E
- [ ] أعرف إزاي أختبر Pinia store لوحده
- [ ] أعرف إزاي أختبر إن component عمل emit
- [ ] أقدر أعمل mock لـ function وأتأكد إنها اتنادت
- [ ] بكتب tests بتختبر **اللي المستخدم بيشوفه**، مش تفاصيل الكود

</details>

### أخطاء شائعة

- **إنك تختبر الـ implementation** (اسم ref جوا الـ component). اختبر اللي المستخدم بيشوفه ويعمله.
- **Tests بتعدّي دايمًا.** جرّب تبوّظ الكود وشوف الـ test بيفشل ولا لأ.

> **نصيحة منتور:** مش لازم 100% coverage. ابدأ بـ test للحاجات اللي **لو باظت هتعمل مشكلة كبيرة**: الحسابات، والـ cart، والـ auth.

---

<a id="week-27"></a>

## الأسبوع 27: Performance و Accessibility

**الهدف:** تخلي الأبلكيشن سريع، وكل الناس تقدر تستخدمه.

### المواضيع

**Performance:**
- إزاي Vue بتتتبع التغييرات وبتعمل re-render
- Vue DevTools Performance
- `v-once` و `v-memo`، و `shallowRef`
- `computed` vs method من ناحية الأداء
- Lazy Loading للـ routes والـ components (`defineAsyncComponent`)
- Core Web Vitals: LCP، و INP، و CLS
- Lighthouse
- الصور وحجم الـ Bundle

**Accessibility:**
- ليه الـ a11y مهمة
- Semantic HTML في Vue
- الكيبورد و Focus Management (خصوصًا مع تغيير الـ route)
- ARIA (وإمتى **متستخدموش**)
- Color Contrast و Screen Readers

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Ahmed Saber: Web Accessibility 101](https://www.youtube.com/playlist?list=PLNknCqb-phEjLVnCbtVTJnWYml0zRvt5Y) | 2.5 ساعة |
| الأساسي | [Performance - vuejs.org](https://vuejs.org/guide/best-practices/performance.html) | إنجليزي |
| الأساسي | [Accessibility - vuejs.org](https://vuejs.org/guide/best-practices/accessibility.html) | إنجليزي |
| مرجع | [Learn Performance - web.dev](https://web.dev/learn/performance) · [Web Vitals](https://web.dev/articles/vitals) | |
| مرجع | [Learn Accessibility - web.dev](https://web.dev/learn/accessibility) | |
| أداة | [Lighthouse](https://developer.chrome.com/docs/lighthouse/overview) · [WAVE](https://wave.webaim.org/) | |

### التاسك: Audit وتحسين مشروع

اختار أكبر مشروع عملته في المستوى ده (غالبًا الـ Dashboard أو الـ Cart):

1. شغّل **Lighthouse** (Mobile) وخد Screenshot **قبل**
2. افتح **Vue DevTools** ودوّر على components بتعمل render كتير من غير داعي
3. اعمل **Lazy Loading** للصفحات
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

- [ ] أعرف إزاي Vue بتعرف إن component محتاج يتحدث
- [ ] أعرف إمتى `shallowRef` بيفيد (داتا كبيرة مش هتتعدل جواها)
- [ ] أعرف يعني إيه LCP و INP و CLS
- [ ] أقدر أقرا تقرير Lighthouse وأعرف أبدأ منين
- [ ] الأبلكيشن بتاعي شغال بالكيبورد كله
- [ ] أعرف إن "**No ARIA is better than bad ARIA**"

</details>

### أخطاء شائعة

- **إنك تحسّن من غير ما تقيس.** افتح Lighthouse و DevTools الأول.
- **`<div @click>` بدل `<button>`.** مش هيشتغل بالكيبورد، والـ Screen Reader مش هيعرف إنه زرار.

> **نصيحة منتور:** **قيس قبل ما تحسّن.** أغلب مشاكل الـ performance اللي بتشوفها في مشاريع المبتدئين جاية من صور كبيرة وحاجات بتتحمّل مش محتاجينها، مش من الـ framework.

---

<a id="week-28"></a>

## الأسبوع 28: Nuxt، الأساسيات والـ Routing

**الهدف:** تفهم Nuxt بيضيف إيه على Vue، وتبني صفحات بالـ File-based Routing.

### المواضيع

- يعني إيه Meta-framework، وليه Nuxt
- CSR vs SSR vs SSG
- إنشاء مشروع وفهم هيكل الملفات
- **Pages و Routes** (الـ routing بالملفات)
- Dynamic Routes
- **Layouts** و Components (و Auto-imports)
- `NuxtLink`
- Assets

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Vuejs Wisdom: Nuxt 3 من 1 لـ 6](https://www.youtube.com/watch?v=q3T_NLWcZBo&list=PLzjSlWqF2aTcdEs97QvAU13E07llvv3UO&index=1) | 46 دقيقة |
| الأساسي | [Nuxt: Introduction](https://nuxt.com/docs/getting-started/introduction) | إنجليزي. كمّل منها Installation و Directory Structure و Routing |

> **عن Nuxt 4:** الكورس بـ Nuxt 3، والنسخة الحالية **Nuxt 4**. الفرق الأساسي اللي هيقابلك إن كود الأبلكيشن بقى جوا فولدر `app/` (يعني `app/pages/` بدل `pages/`). أغلب الباقي زي ما هو. لو حاجة مشتغلتش زي الفيديو، الـ docs هي المرجع.

### التاسك: Blog بـ Nuxt

ابدأ مشروع Blog (هتكمله الأسبوع الجاي):

- `/`: الرئيسية، فيها آخر البوستات
- `/blog`: كل البوستات
- `/blog/[slug]`: صفحة البوست
- `/about`
- Layout `default` فيه Navbar و Footer، و Layout `blog` فيه sidebar
- البوستات حاليًا في ملف `data.ts` (array of objects)
- TypeScript و Tailwind

**التسليم:** على الداشبورد: لينك الـ Repo.

### تحدي إضافي

اكتب البوستات كملفات **Markdown** واعرضها باستخدام [Nuxt Content](https://content.nuxt.com/).

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين CSR و SSR و SSG، وإمتى كل واحد مناسب
- [ ] أعرف إزاي الملفات بتتحول لـ routes في Nuxt
- [ ] أعرف يعني إيه Auto-imports، وليه مش محتاج أعمل import لـ `ref` أو للـ components
- [ ] أقدر أعمل dynamic route وآخد الـ params

</details>

### أخطاء شائعة

- **إنك تعمل `vue-router` بإيدك في Nuxt.** Nuxt بيعمل الـ routing لوحده من فولدر `pages`.
- **إنك تستخدم `window` أو `localStorage` في أي حتة.** الكود بيشتغل على السيرفر الأول، وهناك مفيش `window`. استخدمهم جوا `onMounted` أو `<ClientOnly>`.

> **نصيحة منتور:** Nuxt في الأول هيحسسك إن فيه "سحر" كتير (Auto-imports وغيره). اقرا Directory Structure في الـ docs وهتفهم كل حاجة جاية منين.

---

<a id="week-29"></a>

## الأسبوع 29: Nuxt، Data و SEO و Deploy + الشغل مع الـ AI

**الهدف:** تكمّل الـ Blog بداتا حقيقية و SEO وترفعه، وتتعلم إزاي تستخدم الـ AI كأداة شغل حقيقية.

### المواضيع

**Nuxt:**
- **Data Fetching:** `useFetch` و `useAsyncData`
- Server Routes (`server/api/`)
- **SEO و Meta** (`useSeoMeta`، و `useHead`)
- Transitions
- Plugins و Modules
- صفحة الخطأ
- **Middleware** (حماية الصفحات)
- `useCookie` و `useState`
- Deploy

**الشغل مع الـ AI:**
- إزاي تكتب prompt كويس لمهمة برمجية (السياق، والقيود، والمطلوب بالظبط)
- استخدامه في: الـ boilerplate، والـ tests، وشرح كود مش فاهمه، و code review
- **إزاي تراجع كود الـ AI:** متقبلش حاجة مش فاهمها، واختبر كل حاجة
- الحاجات اللي الـ AI بيغلط فيها كتير: APIs قديمة (Vue 2 و Options API و Nuxt 2)، و packages مش موجودة، وحلول أعقد من اللازم

### المصادر

| النوع | المصدر | المدة |
| :--- | :--- | :---: |
| الأساسي | [Vuejs Wisdom: Nuxt 3 من 7 لـ 13](https://www.youtube.com/watch?v=20WedKm6mcM&list=PLzjSlWqF2aTcdEs97QvAU13E07llvv3UO&index=7) | ساعة |
| مرجع | [Nuxt Docs](https://nuxt.com/docs/getting-started/introduction): Data Fetching، و SEO and Meta، و Deployment | |
| مرجع | [GitHub Copilot Docs](https://docs.github.com/en/copilot) | |

### التاسك: تكملة الـ Blog + Deploy

- البوستات تيجي من API (مثلًا [DummyJSON Posts](https://dummyjson.com/)) بـ `useFetch`
- Server Route واحد على الأقل (`server/api/...`)
- **SEO:** `useSeoMeta` لكل صفحة، وdynamic meta لصفحة البوست (العنوان والوصف من البوست نفسه)
- صفحة خطأ مخصصة (`error.vue`)
- صفحة `/dashboard` محمية بـ **Route Middleware**
- Transitions بين الصفحات
- **Deploy** على Vercel أو Netlify
- Lighthouse SEO و Performance **90+**

**مهمة الـ AI:**
استخدم أي أداة AI عشان:
1. تكتب tests لـ component واحد
2. تعمل review لملف من ملفاتك
3. تشرحلك حاجة في Nuxt مكنتش فاهمها

واكتب في ملف `AI_LOG.md`: كتبت إيه بالظبط (الـ prompt)، وهو رد بإيه، و**إيه اللي كان غلط أو محتاج تعديل في رده**.

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live + ملف `AI_LOG.md`.

<details>
<summary><b>Checklist آخر الأسبوع</b></summary>

<br />

- [ ] أعرف الفرق بين `useFetch` و `$fetch`، وليه `$fetch` لوحده جوا الـ setup ممكن يعمل request مرتين
- [ ] أعرف الكود بيشتغل فين: Server ولا Client ولا الاتنين
- [ ] أقدر أعمل Server Route
- [ ] أعرف إزاي أعمل SEO meta ديناميك
- [ ] رفعت مشروع Nuxt Live
- [ ] بقدر أراجع كود الـ AI وأمسك غلطه

</details>

### أخطاء شائعة

- **`$fetch` في الـ setup بدل `useFetch`.** هيتعمل request على السيرفر وتاني على الـ client.
- **إنك تطلب من الـ AI "اعملّي blog بـ Nuxt".** ممكن يطلعلك كود Nuxt 2 أو Options API. ادّيله سياق: النسخة، و Composition API، والملف اللي إنت فيه، والمطلوب بالظبط.

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
| **التقنيات** | **Nuxt** أو **Vue + Vite**، و TypeScript، و Tailwind |
| **الصفحات** | 5 صفحات على الأقل، منهم dynamic routes |
| **State** | Pinia للـ Client State، و TanStack Query (أو `useFetch` في Nuxt) للـ Server State |
| **Auth** | Login و Register (ممكن وهمي أو بـ API زي DummyJSON)، و Protected Routes |
| **Forms** | فورم واحد معقد على الأقل بـ validation |
| **Testing** | 10 tests على الأقل (Unit + Component) |
| **Performance** | Lighthouse **90+** في الأربع خانات |
| **Accessibility** | شغال بالكيبورد بالكامل |
| **Responsive** | Mobile First |
| **Git** | Branches و Pull Requests، و commits واضحة |
| **Deploy** | Live على Vercel أو Netlify |
| **README** | Screenshots أو GIF، ولينك Live، والتقنيات وليه اخترتها، وإزاي تشغّله، والتحديات اللي قابلتك، وإيه اللي هتضيفه لو عندك وقت |

**التسليم:** على الداشبورد: لينك الـ Repo + لينك الـ Live + فيديو Demo (2-3 دقايق) بتشرح فيه المشروع.

<details>
<summary><b>Checklist آخر الرودماب</b></summary>

<br />

- [ ] أقدر أبني أبلكيشن Vue أو Nuxt كامل من الصفر لوحدي
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

1. **Portfolio:** اعمل موقع شخصي بـ Nuxt فيه مشاريعك
2. **Open Source:** Vue و Nuxt مجتمعاتهم مرحبة جدًا بالمساهمين الجداد، فدوّر على issues عليها `good first issue`
3. **اتعلم Backend بسيط:** Server Routes في Nuxt مع Database، أو Laravel لو حابب (Vue و Laravel ثنائي مشهور جدًا)
4. **قدّم على Internships** حتى لو حاسس إنك مش جاهز. إنت جاهز أكتر ما إنت فاكر.
5. **علّم غيرك:** اكتب بوست عن حاجة اتعلمتها، أو ساعد حد في المستوى الأول. **مفيش طريقة تتعلم بيها أحسن من إنك تشرح.**

**[الرجوع للخريطة](README.md)**

</div>
