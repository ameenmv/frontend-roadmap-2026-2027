<a id="top"></a>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:CA8A04,100:EAB308&height=200&section=header&text=Level%202%20%C2%B7%20Intermediate&fontSize=52&fontColor=ffffff&fontAlignY=38&animation=fadeIn&desc=JavaScript%20%C2%B7%20DOM%20%C2%B7%20Async%20%C2%B7%20Tooling%20%C2%B7%20TypeScript&descSize=18&descAlignY=60" width="100%" alt="Level 2 Intermediate" />

<img src="https://skillicons.dev/icons?i=js,ts,nodejs,npm,vite,git,github" alt="JavaScript TypeScript Node npm Vite Git GitHub" />

<br /><br />

<img src="https://img.shields.io/badge/Weeks-9_→_18-CA8A04?style=for-the-badge" alt="Weeks 9-18" />
<img src="https://img.shields.io/badge/Video-~23_h-EAB308?style=for-the-badge" alt="About 23 hours of video" />
<img src="https://img.shields.io/badge/Main_Source-Elzero_Web_School-111827?style=for-the-badge" alt="Elzero Web School" />

<br /><br />

[Roadmap](README.md) · [Beginner](01-beginner.md) · **Intermediate** · [React](03-react.md) · [Vue](03-vue.md) · [Tracker](TRACKER.md)

</div>

---

If HTML is the skeleton and CSS is the skin, **JavaScript is the brain.**

This is **the most important level** in the roadmap. Everything you do in React or Vue later *is* JavaScript. Strong JS makes frameworks easy; weak JS makes every error a mystery. That's why this level gets **10 weeks**, the longest of all.

| Week | Topic | You ship |
| :--: | :-- | :-- |
| [9](#week-9) | JavaScript basics | A set of problems |
| [10](#week-10) | Arrays, loops, functions, scope | A grade calculator |
| [11](#week-11) | Higher-order functions, objects, destructuring | Student data analysis |
| [12](#week-12) | DOM, BOM, Local Storage | An expense tracker |
| [13](#week-13) | Map, Set, dates, modules | A modular to-do app |
| [14](#week-14) | Async JavaScript & Fetch | A weather app |
| [15](#week-15) | How JavaScript works inside | A quiz app with classes |
| [16](#week-16) | npm, Vite, Git branching | Weather app on Vite + PRs |
| [17](#week-17) | TypeScript | Weather app in TypeScript |
| [18](#week-18) | **Project 2** | An API-driven app in TS |

> [!NOTE]
> The Elzero JavaScript course is 19.5 h across 188 videos. We follow it mostly in order over 7 weeks, then TypeScript. Every part has assignments on the [study plan](https://elzero.org/study/javascript-bootcamp-2021-study-plan/).

---

<a id="week-9"></a>

## Week 9 · JavaScript Basics

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=GM6dQBmc-Xg&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=1"><img src="https://img.youtube.com/vi/GM6dQBmc-Xg/mqdefault.jpg" width="320" alt="Elzero JavaScript #001" /></a>
<br /><b>Elzero · JavaScript #001 → #039</b>
<br />4 h

</td>
<td valign="top">

**Watch:** [Elzero · JavaScript #001 → #039](https://www.youtube.com/watch?v=GM6dQBmc-Xg&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=1) · **4 h**

**Goal:** write small programs with variables, operators, and conditions, and read the Console.

**Topics:** where JS runs (`<script>`, `defer`) · console · data types & `typeof` · `var` / `let` / `const` · strings & template literals · operators & type coercion · numbers & `Math` · string methods · comparison & logic · `if`, ternary, `??`, `switch`

**Practice:** Elzero [01-09](https://elzero.org/javascript-bootcamp-assignments-lesson-from-001-to-009/) · [10-17](https://elzero.org/javascript-bootcamp-assignments-lesson-from-010-to-017/) · [18-22](https://elzero.org/javascript-bootcamp-assignments-lesson-from-018-to-022/) · [23-26](https://elzero.org/javascript-bootcamp-assignments-lesson-from-023-to-026/) · [27-30](https://elzero.org/javascript-bootcamp-assignments-lesson-from-027-to-030/) · [31-32](https://elzero.org/javascript-bootcamp-assignments-lesson-from-031-to-032/) · [33-37](https://elzero.org/javascript-bootcamp-assignments-lesson-from-033-to-037/) · [38-39](https://elzero.org/javascript-bootcamp-assignments-lesson-from-038-to-039/)

**Read:** **[javascript.info](https://javascript.info)** (the best written JS reference) · [JS Guide · MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)

</td>
</tr>
</table>

#### Task · Problem set

In `week-9.js`, one function per problem, results printed to the Console:

1. **BMI** from weight and height, with a category
2. **Even or odd**, with an error message for non-numbers
3. **Largest of three** without `Math.max`
4. **Celsius ↔ Fahrenheit**
5. **Letter grade** (A-F) from a score, using `switch`
6. **Palindrome** check (`level`, `racecar`)
7. **Capitalize** `"hello world"` → `"Hello World"`

> [!TIP]
> **Bonus:** a number-guessing game with `prompt` and `alert`. The computer picks 1-100 and answers "higher" or "lower". You'll need a loop, so peek at the first loops video.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know why `const` is the default, when to use `let`, and why not `var`
- [ ] I know `==` vs `===`
- [ ] I know why `"5" + 3` is `"53"` but `"5" - 3` is `2`
- [ ] I know `||` vs `??`
- [ ] I can list JavaScript's falsy values (there are 8)

</details>

> [!WARNING]
> **Pitfalls:** watching without typing (JS can't be learned by watching) · ignoring red in the Console. An error is a message telling you exactly where to look.

> [!NOTE]
> **Mentor tip:** this week looks easy. Don't rush it. Type coercion and falsy values are behind half the weird bugs you'll ever hit.

<div align="right"><a href="#top">Top ↑</a> · <a href="#week-10">Week 10 →</a></div>

---

<a id="week-10"></a>

## Week 10 · Arrays, Loops, Functions & Scope

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=MLVJhya1CV0&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=40"><img src="https://img.youtube.com/vi/MLVJhya1CV0/mqdefault.jpg" width="320" alt="Elzero JavaScript #040" /></a>
<br /><b>Elzero · JavaScript #040 → #070</b>
<br />3 h

</td>
<td valign="top">

**Watch:** [Elzero · JavaScript #040 → #070](https://www.youtube.com/watch?v=MLVJhya1CV0&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=40) · **3 h**

**Goal:** work with lists of data, repeat work, and split code into clean functions.

**Topics:** arrays (add, remove, search, sort, `slice` vs `splice`) · `for`, `for...of`, `while`, `break`, `continue` · functions, `return`, default & rest params · anonymous & arrow functions · **scope**: global, local, block, lexical

**Practice:** Elzero [40-47](https://elzero.org/javascript-bootcamp-assignments-lesson-from-040-to-047/) · [48-53](https://elzero.org/javascript-bootcamp-assignments-lesson-from-048-to-053/) · [54-56](https://elzero.org/javascript-bootcamp-assignments-lesson-from-054-to-056/) · [57-63](https://elzero.org/javascript-bootcamp-assignments-lesson-from-057-to-063/) · [64-70](https://elzero.org/javascript-bootcamp-assignments-lesson-from-064-to-070/) · [30 Days of JavaScript](https://github.com/Asabeneh/30-Days-Of-JavaScript) (days 5-7)

**Read:** [Functions](https://javascript.info/function-basics) · [Arrays](https://javascript.info/array) · javascript.info

</td>
</tr>
</table>

#### Task · Grade calculator

An array of 10 students, each `[name, grade]`. Write:

1. `getAverage(students)`
2. `getTopStudent(students)`
3. `getFailed(students)`: grades under 50
4. `sortByGrade(students)`: descending, **without mutating the original**
5. `printReport(students)`: a nicely formatted Console report with grades and letters

**No `map`, `filter`, or `reduce` yet.** Loops only.

> [!TIP]
> **Bonus:** print a star pyramid with any number of rows.
> ```text
>    *
>   ***
>  *****
> ```

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know `slice` vs `splice`, and which one mutates
- [ ] I know `for...of` vs `for...in`
- [ ] I know returning a value vs printing it
- [ ] I know how arrow functions differ from regular functions, at least in syntax
- [ ] I know what block scope means

</details>

> [!WARNING]
> **Pitfalls:** functions that do five things · a missing `return`, so you get `undefined` · names like `x`, `arr`, `temp`.

> [!NOTE]
> **Mentor tip:** wrote the same code twice? It should be a function.

<div align="right"><a href="#week-9">← Week 9</a> · <a href="#top">Top ↑</a> · <a href="#week-11">Week 11 →</a></div>

---

<a id="week-11"></a>

## Week 11 · Higher-Order Functions, Objects & Destructuring

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=hTUsHXxEvHc&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=71"><img src="https://img.youtube.com/vi/hTUsHXxEvHc/mqdefault.jpg" width="320" alt="Elzero JavaScript #071" /></a>
<br /><b>Elzero · JavaScript #071 → #085</b>
<br />1.5 h

</td>
<td valign="top">

**Watch:** [Elzero · JavaScript #071 → #085](https://www.youtube.com/watch?v=hTUsHXxEvHc&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=71) · **1.5 h**

**Goal:** handle real data (arrays of objects) the way professional frontend devs do.

**Topics:** **`map`, `filter`, `reduce`, `forEach`** · objects, dot vs bracket notation, nesting · intro to `this` · `Object.create` & `Object.assign` · **destructuring** · **spread** `...`

**Also watch:** [Elzero · Destructuring #115 → #122](https://www.youtube.com/watch?v=tR6VARwdmzA&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=115) + [Spread #132](https://www.youtube.com/watch?v=D9UdBHoAOzg&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=132) · 44 min

**Practice:** Elzero [71-78](https://elzero.org/javascript-bootcamp-assignments-lesson-from-071-to-078/) · [79-85](https://elzero.org/javascript-bootcamp-assignments-lesson-from-079-to-085/) · [115-122](https://elzero.org/javascript-bootcamp-assignments-lesson-from-115-to-122/)

**Read:** [Array methods](https://javascript.info/array-methods) · [Destructuring](https://javascript.info/destructuring-assignment) · javascript.info

</td>
</tr>
</table>

#### Task · Student data analysis

```js
const students = [
  { id: 1, name: "Ahmed", age: 20, track: "frontend", grades: [85, 90, 78], active: true },
  { id: 2, name: "Sara", age: 21, track: "backend", grades: [92, 88, 95], active: true },
  { id: 3, name: "Omar", age: 19, track: "frontend", grades: [60, 45, 70], active: false },
  // ...15 students total
];
```

Using **only `map`, `filter`, `reduce`** (no plain loops):

1. Names of active students
2. Each student with an `average` field (new objects)
3. Count per track `{ frontend: 6, backend: 5 }` with `reduce`
4. Top student per track
5. A greeting function that destructures `{ name, track }` in its parameters
6. Add a student **without mutating** the array (spread)

> [!TIP]
> **Bonus:** write your own `myMap` and `myFilter` without using the built-ins.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know `map` vs `forEach`
- [ ] I can write a `reduce` without looking
- [ ] I know when to use `obj.key` vs `obj[key]`
- [ ] I know spread makes a **shallow** copy, and what that means
- [ ] Destructured code doesn't confuse me anymore

</details>

> [!WARNING]
> **Pitfalls:** an arrow function with `{}` but no `return` inside `map` gives you an array of `undefined` · mutating the original object inside `map`. In React and Vue, not mutating is the law.

> [!NOTE]
> **Mentor tip:** you'll write `map`, `filter`, `reduce`, destructuring, and spread **every day** in React and Vue. If this week isn't 100% clear, take two extra days.

<div align="right"><a href="#week-10">← Week 10</a> · <a href="#top">Top ↑</a> · <a href="#week-12">Week 12 →</a></div>

---

<a id="week-12"></a>

## Week 12 · DOM, BOM & Local Storage

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=AOabnOI4vOQ&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=86"><img src="https://img.youtube.com/vi/AOabnOI4vOQ/mqdefault.jpg" width="320" alt="Elzero JavaScript #086" /></a>
<br /><b>Elzero · JavaScript #086 → #114</b>
<br />3.5 h

</td>
<td valign="top">

**Watch:** [Elzero · JavaScript #086 → #114](https://www.youtube.com/watch?v=AOabnOI4vOQ&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=86) · **3.5 h**

**Goal:** make pages interactive: add and remove elements, respond to clicks, and keep data after the browser closes.

**Topics:** **DOM** (select, read/write content & attributes, create, append, remove) · **events** (`addEventListener`, form validation, `preventDefault`) · `classList` · DOM traversal · **BOM** (`setTimeout`, `setInterval`, `location`, `history`, scroll) · **Local** & Session Storage

**Build one:** Elzero [Tabs](https://www.youtube.com/watch?v=pnLm4ga_P6k&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=27) · [Image Slider](https://www.youtube.com/watch?v=QmPXb-RHy5s&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=7) · [Countdown Timer](https://www.youtube.com/watch?v=eFsiOTJrrE8&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=16)

**Practice:** Elzero [86-93](https://elzero.org/javascript-bootcamp-assignments-lesson-from-086-to-093/) · [94-101](https://elzero.org/javascript-bootcamp-assignments-lesson-from-094-to-101/) · [102-110](https://elzero.org/javascript-bootcamp-assignments-lesson-from-102-to-110/) · [111-114](https://elzero.org/javascript-bootcamp-assignments-lesson-from-111-to-114/)

**Read:** [Intro to the DOM · MDN](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction) · [localStorage · MDN](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage)

</td>
</tr>
</table>

#### Task · Expense tracker

- A form: description, amount, category (food, transport, courses...), date
- **Validation** with errors shown **in the page**, not `alert`
- A list of expenses with a delete button each
- A **total** that updates automatically
- Filter by category (`select`)
- **Everything persists in Local Storage.** Refresh and it's still there.

> [!TIP]
> **Bonus:** an **edit** button · **event delegation**: one listener on the list instead of one per button.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know `querySelector` vs `querySelectorAll` and what each returns
- [ ] I know `innerHTML` vs `textContent`, and why `innerHTML` can be dangerous
- [ ] I know what event delegation is and why it helps
- [ ] I know Local Storage only stores strings, and how to store arrays and objects
- [ ] I know Local vs Session Storage

</details>

> [!WARNING]
> **Pitfalls:** putting user input into `innerHTML` (someone types `<img src=x onerror=alert(1)>` and it runs) · treating the DOM as your data. Keep **an array in JS** as the source of truth and redraw from it. That's exactly what React and Vue do.

> [!NOTE]
> **Mentor tip:** get "**data in an array, UI drawn from it**" this week and you already understand half of React and Vue.

<div align="right"><a href="#week-11">← Week 11</a> · <a href="#top">Top ↑</a> · <a href="#week-13">Week 13 →</a></div>

---

<a id="week-13"></a>

## Week 13 · Map, Set, Dates & Modules

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=lsirOGbdWYA&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=123"><img src="https://img.youtube.com/vi/lsirOGbdWYA/mqdefault.jpg" width="320" alt="Elzero JavaScript #123" /></a>
<br /><b>Elzero · JavaScript #123 → #133</b>
<br />1.5 h

</td>
<td valign="top">

**Watch:** [Elzero · JavaScript #123 → #133](https://www.youtube.com/watch?v=lsirOGbdWYA&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=123) · **1.5 h**

**Goal:** use modern JS tools and organize your code across files.

**Topics:** **Set** & **Map** (and when to use them over arrays and objects) · WeakSet & WeakMap · `Array.from`, `some`, `every` · dates & times · generators (intro) · **ES modules**: `import` / `export`, named vs default

**Also watch:** [Elzero · Dates, generators & modules #159 → #168](https://www.youtube.com/watch?v=G5Ql9pQFxJA&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=159) · 51 min

**Build first:** [Elzero · To-Do App with Local Storage](https://www.youtube.com/watch?v=ylsFXMHpFUQ&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=22)

**Practice:** Elzero [123-133](https://elzero.org/javascript-bootcamp-assignments-lesson-from-123-to-133/) · [159-168](https://elzero.org/javascript-bootcamp-assignments-lesson-from-159-to-168/)

**Read:** [JavaScript modules · MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules)

</td>
</tr>
</table>

#### Task · Modular to-do app

```text
todo-app/
├── index.html
├── css/style.css
└── js/
    ├── main.js      → entry point
    ├── storage.js   → save / load
    ├── todos.js     → add, remove, toggle, edit
    └── ui.js        → render the list
```

- Add, delete, complete, and edit tasks
- Filters: all, active, done
- An "X tasks left" counter
- A readable creation date ("3 hours ago" or "Nov 13")
- `<script type="module">`

> [!TIP]
> **Bonus:** drag & drop to reorder (HTML Drag and Drop API) · watch [Regex #134 → #146](https://www.youtube.com/watch?v=V-8vs_teVlo&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=134) (1 h) and validate task titles.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know when to use `Set` (unique values) and `Map` (any-type keys)
- [ ] I know `export default` vs `export`
- [ ] I know why modules fail when opened by double-click
- [ ] Each file in my project has one clear job

</details>

> [!WARNING]
> **Pitfalls:** a 500-line `main.js` · circular imports (`a.js` imports `b.js`, which imports `a.js`).

> [!NOTE]
> **Mentor tip:** how you split files today is how you'll split components tomorrow. Ask, "what is this file responsible for?"

<div align="right"><a href="#week-12">← Week 12</a> · <a href="#top">Top ↑</a> · <a href="#week-14">Week 14 →</a></div>

---

<a id="week-14"></a>

## Week 14 · Async JavaScript & Fetch

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=VA_AROETZ58&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=169"><img src="https://img.youtube.com/vi/VA_AROETZ58/mqdefault.jpg" width="320" alt="Elzero JavaScript #169" /></a>
<br /><b>Elzero · JavaScript #169 → #188</b>
<br />2 h

</td>
<td valign="top">

**Watch:** [Elzero · JavaScript #169 → #188](https://www.youtube.com/watch?v=VA_AROETZ58&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=169) · **2 h**

**Goal:** fetch real data from the internet and show it on your page.

**Topics:** JSON · what an API is · sync vs async · **call stack, Web APIs, event loop** · AJAX & XHR (for understanding) · callback hell · **Promises** · **Fetch** · `Promise.all` / `allSettled` / `race` · **async / await** · `try / catch`

**Build one:** Elzero [GitHub Repos Fetcher](https://www.youtube.com/watch?v=uCKCSO8vkiU&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=6) · [Currency API](https://www.youtube.com/watch?v=wZ90BnBbRsg&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=4)

**Practice:** Elzero [169-178](https://elzero.org/javascript-bootcamp-assignments-lesson-from-169-to-178/) · [179-188](https://elzero.org/javascript-bootcamp-assignments-lesson-from-179-to-188/)

**Read:** [Using Fetch · MDN](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) · [Async JS · MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Async_JS) · [Event loop · javascript.info](https://javascript.info/event-loop)

</td>
</tr>
</table>

#### Task · Weather app

Use [Open-Meteo](https://open-meteo.com/) (free, no API key):

- Type a city → geocode it → fetch the weather
- Current temperature, conditions, humidity, wind, and a 7-day forecast
- **Three clear states:** loading (spinner), error (city not found / offline), success
- `async / await` + `try / catch` only, no `.then`
- Remember the last city in Local Storage

> [!TIP]
> **Bonus:** a "**my location**" button with `navigator.geolocation` · **debounce** the input (wait 500 ms after typing stops).

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I can draw the event loop for someone who doesn't get it
- [ ] I know why code after `setTimeout(fn, 0)` runs first
- [ ] I know `fetch` **doesn't** throw on 404 or 500, and how to check `response.ok`
- [ ] I know `Promise.all` vs `Promise.allSettled`
- [ ] I can inspect requests and responses in the Network tab

</details>

> [!WARNING]
> **Pitfalls:** a missing `await`, so you get `Promise {<pending>}` · no error handling (networks fail, APIs go down, users typo) · no loading state, so users click 10 times.

> [!NOTE]
> **Mentor tip:** async trips up everyone. Watch the event loop videos twice and draw it on paper. It clicks.

<div align="right"><a href="#week-13">← Week 13</a> · <a href="#top">Top ↑</a> · <a href="#week-15">Week 15 →</a></div>

---

<a id="week-15"></a>

## Week 15 · How JavaScript Works Inside

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=uv5OULDiCXg&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=147"><img src="https://img.youtube.com/vi/uv5OULDiCXg/mqdefault.jpg" width="320" alt="Elzero JavaScript #147" /></a>
<br /><b>Elzero · JavaScript OOP #147 → #158</b>
<br />1 h

</td>
<td valign="top">

**Watch:** [Elzero · JavaScript OOP #147 → #158](https://www.youtube.com/watch?v=uv5OULDiCXg&list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv&index=147) · **1 h**

**Goal:** understand what happens behind the curtain: closures, `this`, prototypes, classes. The stuff every interview asks.

**Topics:** constructor functions & **classes** · static, inheritance (`extends`, `super`), private fields (`#`) · **prototype chain** · property descriptors · **closures** · **`this`** in every context, `call` / `apply` / `bind` · hoisting

**Must read:** **[Closures · javascript.info](https://javascript.info/closure)**

**Build first:** [Elzero · Quiz App](https://www.youtube.com/watch?v=T5QyLcmcMJ4&list=PLDoPjvoNmBAycCXz5d9WvqlmykUIys5e8&index=5)

**Practice:** Elzero [147-158](https://elzero.org/javascript-bootcamp-assignments-lesson-from-147-to-158/)

**Read:** [Closures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures) · [this](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this) · [Prototype chain](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain) · MDN

</td>
</tr>
</table>

#### Task · Quiz app with classes

A JavaScript quiz with questions you write:

- `class Question`: text, choices, answer, `isCorrect(answer)`
- `class Quiz`: questions, current index, score, `next()`, `answer()`, `isFinished()`
- `class QuizUI`: rendering only
- A 15-second **timer** per question, built with a **closure**
- A results screen showing right and wrong answers
- High score saved in Local Storage

> [!TIP]
> **Bonus:** `createCounter()` returning `increment`, `decrement`, `getValue`, where the count is **impossible** to reach from outside. A classic interview question.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I can explain a closure with my own example
- [ ] I know what `this` points to in each of the four cases
- [ ] I know why arrow functions have no `this` of their own
- [ ] I know `class` is nicer syntax over prototypes
- [ ] I know hoisting and how `var` and `let` differ there

</details>

> [!WARNING]
> **Pitfalls:** memorizing the closure definition without being able to write one · god classes. One class, one job.

> [!NOTE]
> **Mentor tip:** every frontend interview asks about closures, `this`, and the event loop. Come back to this week before every interview.

<div align="right"><a href="#week-14">← Week 14</a> · <a href="#top">Top ↑</a> · <a href="#week-16">Week 16 →</a></div>

---

<a id="week-16"></a>

## Week 16 · npm, Vite & Git Branching

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=n43bagVuJPU&list=PLDoPjvoNmBAw4eOj58MZPakHjaO3frVMF&index=10"><img src="https://img.youtube.com/vi/n43bagVuJPU/mqdefault.jpg" width="320" alt="Elzero Git #10" /></a>
<br /><b>Elzero · Git #07-08 + #10 → #20</b>
<br />1.5 h

</td>
<td valign="top">

**Watch:** [Elzero · Git #07-08 + #10 → #20](https://www.youtube.com/watch?v=n43bagVuJPU&list=PLDoPjvoNmBAw4eOj58MZPakHjaO3frVMF&index=10) · **1.5 h**

**Goal:** work the way companies do: a Vite project, npm packages, branches, and pull requests.

**Topics:** Node & npm, `package.json`, dependencies vs devDependencies, scripts · why bundlers exist · **Vite** (`create`, `dev`, `build`, `import.meta.env`) · ESLint & Prettier · Git config & SSH keys · **branching & merging** · **pull requests** · stash, restore, reset · `.gitignore` · tags & releases

**Play:** **[Learn Git Branching](https://learngitbranching.js.org/)** (the best way to *see* branches)

**Read:** [Vite guide](https://vite.dev/guide/) · [About npm](https://docs.npmjs.com/about-npm) · [Pro Git book](https://git-scm.com/book/en/v2)

</td>
</tr>
</table>

#### Task · Move the weather app to Vite + PRs

1. New Vite project (vanilla JS); move your week 14 weather app in
2. Split it into modules
3. Install and use an npm package (e.g. [`dayjs`](https://www.npmjs.com/package/dayjs) for dates)
4. Set up ESLint and Prettier
5. **All work on branches** (`feature/vite-setup`, `feature/forecast`...), each merged through a **pull request** with a description
6. Auto-deploy to Vercel or Netlify on every push to `main`

**Submit** the repo (3+ PRs visible) and the live link.

> [!TIP]
> **Bonus:** finish the Main levels of Learn Git Branching · create a merge conflict on purpose and resolve it.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know what's in `package.json`
- [ ] I know why `node_modules` isn't committed, and how others install deps
- [ ] I know `npm run dev` vs `npm run build`
- [ ] I can branch, work, open a PR, and merge
- [ ] I can resolve a simple merge conflict

</details>

> [!WARNING]
> **Pitfalls:** committing `node_modules` · API keys in code (use `.env` and `.gitignore` it; and remember **nothing in frontend code is truly secret**) · working directly on `main`.

> [!NOTE]
> **Mentor tip:** day one at any company: "here's the repo, make a branch, open a PR." People who can do that on day one stand out.

<div align="right"><a href="#week-15">← Week 15</a> · <a href="#top">Top ↑</a> · <a href="#week-17">Week 17 →</a></div>

---

<a id="week-17"></a>

## Week 17 · TypeScript

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=yUndnE-2osg&list=PLDoPjvoNmBAy532K9M_fjiAmrJ0gkCyLJ&index=1"><img src="https://img.youtube.com/vi/yUndnE-2osg/mqdefault.jpg" width="320" alt="Elzero TypeScript #01" /></a>
<br /><b>Elzero · TypeScript #01 → #38</b>
<br />3.5 h

</td>
<td valign="top">

**Watch:** [Elzero · TypeScript #01 → #38](https://www.youtube.com/watch?v=yUndnE-2osg&list=PLDoPjvoNmBAy532K9M_fjiAmrJ0gkCyLJ&index=1) · **3.5 h**

**Goal:** write JavaScript with types, so mistakes get caught as you type, not by your users.

**Topics:** why TS · `tsconfig` & strict mode · annotations · `any` vs `unknown` · **type aliases & interfaces** · literal, **union** & intersection types · tuples, enums, `void`, `never` · assertions · TS classes & access modifiers · **generics**

**Practice:** Elzero [01-11](https://elzero.org/typescript-assignments-lessons-from-1-to-11/) · [12-21](https://elzero.org/typescript-assignments-lessons-from-12-to-21/) · [22-31](https://elzero.org/typescript-assignments-lessons-from-22-to-31/) · [32-38](https://elzero.org/typescript-assignments-lessons-from-32-to-38/) · [Total TypeScript beginner exercises](https://www.totaltypescript.com/tutorials/beginners-typescript)

**Read:** [TS Handbook](https://www.typescriptlang.org/docs/handbook/intro.html) · [TS Playground](https://www.typescriptlang.org/play)

</td>
</tr>
</table>

> [!NOTE]
> Elzero uses `tsc` directly, which is great for learning. In real projects Vite handles TS for you: `npm create vite@latest` → **Vanilla + TypeScript**.

#### Task · Weather app in TypeScript

- `strict: true`
- **Zero `any`** in the whole project
- An `interface` or `type` for every API response
- Typed parameters and return values on every function
- At least one generic, e.g. `fetchJson<T>(url: string): Promise<T>`
- `npm run build` passes with no errors

> [!TIP]
> **Bonus:** model page state as a **discriminated union** and watch TS stop you from reading `data` while `loading`.
> ```ts
> type State =
>   | { status: "loading" }
>   | { status: "success"; data: Weather }
>   | { status: "error"; message: string };
> ```

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know `type` vs `interface`
- [ ] I know `any` vs `unknown`
- [ ] I can write a simple generic function
- [ ] I know TS disappears at build time and gives no runtime safety
- [ ] I can read a TS error and understand it

</details>

> [!WARNING]
> **Pitfalls:** `as any` to silence errors (that's unplugging the smoke alarm) · annotating what TS already infers (`const name: string = "Ahmed"`).

> [!NOTE]
> **Mentor tip:** week one with TS feels slow and nagging. Two weeks later you won't want to write JS without it.

<div align="right"><a href="#week-16">← Week 16</a> · <a href="#top">Top ↑</a> · <a href="#week-18">Week 18 →</a></div>

---

<a id="week-18"></a>

## Week 18 · Project 2: API App in TypeScript

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:CA8A04,100:EAB308&height=90&text=Milestone%20Project%202&fontSize=34&fontColor=ffffff&animation=twinkling" width="100%" alt="Milestone Project 2" />

</div>

**Goal:** build a complete app on a real API, with TypeScript and Vite, on your own.

| Idea | API | Level |
| :-- | :-- | :--: |
| **Movies Explorer**: search, details, favorites | [TMDB](https://www.themoviedb.org/documentation/api) (free key) | ●●○ |
| **Countries Explorer**: search, filter by region, neighbors | [REST Countries](https://restcountries.com/) | ●●○ |
| **Mini Store**: products, search, filters, cart | [DummyJSON](https://dummyjson.com/) | ●●● |
| **GitHub Profile Finder**: profile, repos, top languages | [GitHub REST API](https://docs.github.com/en/rest) | ●●● |
| **Your idea** | Any public API | Talk to your mentor |

| Requirement | Details |
| :-- | :-- |
| **Stack** | Vite + TypeScript (`strict`) + CSS or Tailwind. **No frameworks.** |
| **Pages** | A list view + a details page or modal |
| **Search & filter** | Debounced search + at least one filter |
| **States** | Loading, error, and empty ("no results") |
| **Persistence** | Favorites, cart, or last search in Local Storage |
| **Structure** | `api/`, `ui/`, `types/`, `utils/` |
| **Responsive** | Works well on phones |
| **Git** | Branches + PRs, no direct commits to `main` |
| **Deploy** | Vercel or Netlify; API keys in environment variables |
| **README** | Screenshot, live link, stack, how to run, what you learned |

> [!TIP]
> **Bonus:** pagination or infinite scroll · **URL state** (`?q=egypt&region=africa`) so shared links show the same results · persistent dark mode.

<details>
<summary><b>Level 2 exit checklist</b></summary>

<br />

- [ ] I can build a full interactive app in plain JS
- [ ] Async and Promises don't confuse me
- [ ] I split code into modules logically
- [ ] I write TypeScript without `any`
- [ ] Branches and PRs feel normal
- [ ] When a bug appears, I find it with DevTools (Console, Network, Sources)

</details>

> [!WARNING]
> **Pitfalls:** an idea too big to finish (small and complete beats big and half-broken) · building all the UI first. Get the API calls working in the Console, then build the UI.

> [!NOTE]
> **Mentor tip:** you now know more JavaScript than many people who've used React for a year, because most people jump straight to a framework.

<div align="right"><a href="#week-17">← Week 17</a> · <a href="#top">Top ↑</a></div>

---

<div align="center">

### Level 2 done.

You've noticed: as apps grow, updating the UI by hand every time data changes gets painful. That's exactly what React and Vue solve.

**Pick your path** ([not sure?](README.md#levels))

<a href="03-react.md"><img src="https://img.shields.io/badge/React_→_Next.js-0891B2?style=for-the-badge&logo=react&logoColor=white" alt="React track" /></a>
<a href="03-vue.md"><img src="https://img.shields.io/badge/Vue_→_Nuxt-059669?style=for-the-badge&logo=vuedotjs&logoColor=white" alt="Vue track" /></a>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:EAB308,100:CA8A04&height=110&section=footer" width="100%" alt="" />

</div>
