<a id="top"></a>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:059669,100:34D399&height=200&section=header&text=Level%203%20%C2%B7%20Vue&fontSize=56&fontColor=ffffff&fontAlignY=38&animation=fadeIn&desc=Vue%203%20%C2%B7%20Router%20%C2%B7%20Pinia%20%C2%B7%20Testing%20%C2%B7%20Nuxt&descSize=18&descAlignY=60" width="100%" alt="Level 3 Vue" />

<img src="https://skillicons.dev/icons?i=vue,ts,pinia,tailwind,vitest,nuxtjs,vercel" alt="Vue TypeScript Pinia Tailwind Vitest Nuxt Vercel" />

<br /><br />

<img src="https://img.shields.io/badge/Weeks-19_→_30-059669?style=for-the-badge" alt="Weeks 19-30" />
<img src="https://img.shields.io/badge/Video-~15_h-34D399?style=for-the-badge" alt="About 15 hours of video" />
<img src="https://img.shields.io/badge/Vue-3_Composition_API-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D" alt="Vue 3 Composition API" />
<img src="https://img.shields.io/badge/Nuxt-4-00DC82?style=for-the-badge&logo=nuxt&logoColor=white" alt="Nuxt 4" />

<br /><br />

[Roadmap](README.md) · [Beginner](01-beginner.md) · [Intermediate](02-intermediate.md) · [React](03-react.md) · **Vue** · [Tracker](TRACKER.md)

</div>

---

Remember week 12, updating the UI by hand every time data changed? Vue says: **just change the data, I'll update the page.** That's **reactivity**, the heart of Vue.

Vue is known as the easiest framework to start with: templates look like the HTML you know, and its docs are some of the best anywhere. You'll finish with **Nuxt**, which turns Vue into a full framework.

| Week | Topic | You ship |
| :--: | :-- | :-- |
| [19](#week-19) | Template syntax & directives | Landing page in Vue |
| [20](#week-20) | Composition API & components | A multi-step form |
| [21](#week-21) | Lifecycle, watchers, composables, fetching | Movies app |
| [22](#week-22) | Vue Router | A multi-page app |
| [23](#week-23) | Styling & component libraries | A mini UI kit |
| [24](#week-24) | Pinia | A shopping cart |
| [25](#week-25) | TanStack Query | An admin dashboard |
| [26](#week-26) | Testing | Tests for the cart |
| [27](#week-27) | Performance & accessibility | An audit, before & after |
| [28](#week-28) | Nuxt: basics & routing | A blog |
| [29](#week-29) | Nuxt: data, SEO, deploy + AI workflow | The blog, live |
| [30](#week-30) | **Graduation project** | A complete app |

> [!IMPORTANT]
> **Main Arabic source:** the **Vuejs Wisdom** channel: [Vue 3](https://www.youtube.com/playlist?list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV), [Composition API](https://www.youtube.com/playlist?list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC), [Nuxt 3](https://www.youtube.com/playlist?list=PLzjSlWqF2aTcdEs97QvAU13E07llvv3UO). The source of truth is **[vuejs.org](https://vuejs.org/guide/introduction.html)**. Its docs read like a course, so read them.
>
> **Options vs Composition API:** we use **Composition API with `<script setup>`**, the modern default and best with TypeScript. We watch the start of the Options course for templates and directives (identical in both), then switch.
>
> **From now on, every Vue project is TypeScript** (`<script setup lang="ts">`). Stuck? [Vue + TypeScript](https://vuejs.org/guide/typescript/overview.html).

---

<a id="week-19"></a>

## Week 19 · Template Syntax & Directives

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=Vne-X1taBfI&list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV&index=1"><img src="https://img.youtube.com/vi/Vne-X1taBfI/mqdefault.jpg" width="320" alt="Vuejs Wisdom Vue 3 lesson 1" /></a>
<br /><b>Vuejs Wisdom · Vue 3, 1 → 15</b>
<br />2 h

</td>
<td valign="top">

**Watch:** [Vuejs Wisdom · Vue 3, 1 → 15](https://www.youtube.com/watch?v=Vne-X1taBfI&list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV&index=1) · **2 h**

**Goal:** understand how Vue binds data to HTML, and use the core directives.

**Topics:** new project: `npm create vue@latest` (pick TS, Router, Pinia, Vitest, ESLint) · `{{ }}` & `v-bind` (`:`) · `v-on` (`@`) & modifiers · **`v-model`** · computed · dynamic classes & styles · **`v-if` / `v-show`** · **`v-for`** & `:key`

**Interactive:** **[Official Vue tutorial](https://vuejs.org/tutorial/)**: set **Composition** + **SFC** in its settings

**Read:** [Template syntax](https://vuejs.org/guide/essentials/template-syntax.html)

</td>
</tr>
</table>

> [!NOTE]
> The course writes JS with the Options API (`data()`, `methods`). Focus on the **`<template>`** part; that stays the same. You'll write `<script>` in Composition API from next week, and the official tutorial already shows it.

#### Task · Landing page in Vue

Rebuild your week 8 landing page in Vue:

- Repeated content (cards, testimonials, nav links) as **arrays of objects** rendered with `v-for`
- A mobile menu toggled with `v-if` / `v-show`
- Pricing with a **monthly / yearly** toggle (computed prices)
- A newsletter form with `v-model` and simple validation
- Still **one component** this week; we split next week

> [!TIP]
> **Bonus:** finish all 15 steps of the official tutorial.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know `v-if` vs `v-show`
- [ ] I know why `:key` matters with `v-for`
- [ ] I know computed vs method
- [ ] I know what `v-model` does underneath (`:value` + `@input`)
- [ ] I know the shorthands: `:` and `@`

</details>

> [!WARNING]
> **Pitfalls:** `v-if` and `v-for` on the same element (use `<template v-for>` or a filtered computed) · **Vue CLI**: if the course runs `vue create`, use `npm create vue@latest` instead. Vue CLI is in maintenance mode; new projects use Vite.

> [!NOTE]
> **Mentor tip:** if you have time, read the docs' **Essentials** section in order. It answers almost every question you'll have.

<div align="right"><a href="#top">Top ↑</a> · <a href="#week-20">Week 20 →</a></div>

---

<a id="week-20"></a>

## Week 20 · Composition API & Components

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=scY-dpK_Sl8&list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC&index=1"><img src="https://img.youtube.com/vi/scY-dpK_Sl8/mqdefault.jpg" width="320" alt="Vuejs Wisdom Composition API lesson 1" /></a>
<br /><b>Vuejs Wisdom · Composition API 1 → 6 + 8</b>
<br />57 min

</td>
<td valign="top">

**Watch:** [Vuejs Wisdom · Composition API 1 → 6 + 8](https://www.youtube.com/watch?v=scY-dpK_Sl8&list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC&index=1) · **57 min**

**Goal:** write modern Vue and split the app into components that talk to each other.

**Topics:** `<script setup>` · **reactivity**: `ref` vs `reactive` · functions & `computed` · template refs · **single-file components** · **props** (`defineProps<{...}>()`) · **emits** (`defineEmits`) · **slots** · scoped styles

**Also watch:** [Slots, Options course lesson 29](https://www.youtube.com/watch?v=kfFkZGYKZ3w&list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV&index=29) · 11 min

**Read:** [Reactivity fundamentals](https://vuejs.org/guide/essentials/reactivity-fundamentals.html) · [Props](https://vuejs.org/guide/components/props.html) · [Events](https://vuejs.org/guide/components/events.html) · [Slots](https://vuejs.org/guide/components/slots.html)

</td>
</tr>
</table>

#### Task · Multi-step form

A 3-step course application form:

1. **Personal:** name, email, phone
2. **Academic:** college, year, track (radio), skills (checkboxes)
3. **Review:** all data + submit

- Each step is its **own component**; the parent owns the data
- Steps receive data through **props** and report changes through **emits**
- A `BaseInput` using `v-model` (`defineModel`) that shows its error
- A `StepLayout` with a default **slot** for content and a **named slot** for buttons
- A progress bar and per-step validation

> [!TIP]
> **Bonus:** save the form to Local Storage as the user types. You'll need `watch` (peek at next week).

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know `ref` vs `reactive`, and why the docs recommend `ref`
- [ ] I know why `.value` is needed in script but not in templates
- [ ] I know props are **read-only**; children notify parents with emits
- [ ] I know default vs named slots
- [ ] I know what `defineModel` does

</details>

> [!WARNING]
> **Pitfalls:** destructuring a `reactive` object (reactivity lost; use `toRefs` or `ref`) · mutating a prop in a child · forgetting `.value`.

> [!NOTE]
> **Mentor tip:** "**props down, events up**" is the foundation of every framework. Get it and React, Angular, and Svelte feel just as familiar.

<div align="right"><a href="#week-19">← Week 19</a> · <a href="#top">Top ↑</a> · <a href="#week-21">Week 21 →</a></div>

---

<a id="week-21"></a>

## Week 21 · Lifecycle, Watchers, Composables & Fetching

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=0GO4UunMALc&list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC&index=11"><img src="https://img.youtube.com/vi/0GO4UunMALc/mqdefault.jpg" width="320" alt="Vuejs Wisdom Composition API lesson 11" /></a>
<br /><b>Vuejs Wisdom · Composition 11 → 13</b>
<br />24 min

</td>
<td valign="top">

**Watch:** [Vuejs Wisdom · Composition 11 → 13](https://www.youtube.com/watch?v=0GO4UunMALc&list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC&index=11) · **24 min**

**Goal:** load data from an API, share data across distant components, and write logic you can reuse.

**Topics:** **lifecycle hooks** (`onMounted`, `onUnmounted`) · **`watch` & `watchEffect`** · **provide / inject** · `v-model` on components · API requests · loading & error states · **composables**, Vue's way to share logic (like React's custom hooks)

**Also watch:** [v-model & HTTP requests, Options course 31 → 35](https://www.youtube.com/watch?v=0pODnNSy4oI&list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV&index=31) · 1.5 h

**Read:** **[Composables](https://vuejs.org/guide/reusability/composables.html)** (read it all; it has a `useFetch` example) · [Lifecycle](https://vuejs.org/guide/essentials/lifecycle.html) · [Watchers](https://vuejs.org/guide/essentials/watchers.html) · [Provide / Inject](https://vuejs.org/guide/components/provide-inject.html)

</td>
</tr>
</table>

#### Task · Movies app

If your Project 2 was a movies app, rebuild it in Vue. Otherwise build one now with [TMDB](https://www.themoviedb.org/documentation/api) or [DummyJSON](https://dummyjson.com/):

- A list from the API with debounced search (`watch`)
- A **composable** `useFetch<T>(url)` returning `{ data, isLoading, error }` that refetches when a `ref` URL changes
- A `useTheme()` composable for dark mode
- Favorites via **provide / inject**, persisted in Local Storage
- Fast typing never shows a stale result (`AbortController` + `onWatcherCleanup` or the `watch` cleanup)

> [!TIP]
> **Bonus:** `useLocalStorage<T>(key, defaultValue)` returning a `ref` that saves itself on every change.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know `watch` vs `watchEffect` vs `computed`
- [ ] I know where API calls go (setup or `onMounted`)
- [ ] I know when provide / inject fits and when props are better
- [ ] I can write a composable
- [ ] I clean up timers and listeners in `onUnmounted`

</details>

> [!WARNING]
> **Pitfalls:** `watch` to derive a value (that's `computed`) · never cleaning up a `setInterval` or a `window` listener.

> [!NOTE]
> **Mentor tip:** composables are Vue 3's superpower. Wrote the same logic in two components? Ask: "should this be a composable?"

<div align="right"><a href="#week-20">← Week 20</a> · <a href="#top">Top ↑</a> · <a href="#week-22">Week 22 →</a></div>

---

<a id="week-22"></a>

## Week 22 · Vue Router

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=_Ppqm08EUfs&list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV&index=40"><img src="https://img.youtube.com/vi/_Ppqm08EUfs/mqdefault.jpg" width="320" alt="Vuejs Wisdom Vue Router" /></a>
<br /><b>Vuejs Wisdom · Vue Router 40 → 54</b>
<br />2 h

</td>
<td valign="top">

**Watch:** [Vuejs Wisdom · Vue Router 40 → 54](https://www.youtube.com/watch?v=_Ppqm08EUfs&list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV&index=40) · **2 h**

**Goal:** build a multi-page app with no full page reloads.

**Topics:** SPA · routes, `RouterLink`, `RouterView` · hash vs history mode · `router.push` / `replace` / `go` · **dynamic routes**, params & query · **nested routes** · 404 page · **navigation guards** (`beforeEach`) · `useRouter` & `useRoute`

**Also watch:** [Router & Route in Composition API](https://www.youtube.com/watch?v=snhWSqULz0Q&list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC&index=7) · 7 min

**Read:** [Vue Router guide](https://router.vuejs.org/guide/)

</td>
</tr>
</table>

#### Task · Multi-page app

Extend your movies app (or start fresh):

- `/` home · `/movies` list with search & filter **in the URL** (`?q=batman&genre=action`) · `/movies/:id` details · `/favorites`
- `/login` (fake) · `/profile` **protected** by a navigation guard, redirects to `/login`
- A proper 404 page
- A shared layout; the active `RouterLink` is styled (`router-link-active`)

> [!IMPORTANT]
> Refresh on `/movies/5` after deploying gives a 404? Look up "SPA redirect rules" for Netlify or Vercel.

> [!TIP]
> **Bonus:** lazy-load pages with `component: () => import('./views/MovieDetails.vue')` and watch each one load separately in the Network tab.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know `<a>` vs `<RouterLink>`
- [ ] I know `useRouter` vs `useRoute`
- [ ] I know params vs query
- [ ] I can write a navigation guard
- [ ] I know hash vs history mode and why history needs server config

</details>

> [!WARNING]
> **Pitfalls:** going from `/movies/1` to `/movies/2` **reuses** the component. If you only fetch in `onMounted`, the data won't update. Watch the param.

> [!NOTE]
> **Mentor tip:** the URL is the web's oldest and best state manager. Anything a user might share (search, filters, page) belongs in it.

<div align="right"><a href="#week-21">← Week 21</a> · <a href="#top">Top ↑</a> · <a href="#week-23">Week 23 →</a></div>

---

<a id="week-23"></a>

## Week 23 · Styling & Component Libraries

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=QSBs0ceChnI&list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC&index=15"><img src="https://img.youtube.com/vi/QSBs0ceChnI/mqdefault.jpg" width="320" alt="Vuejs Wisdom Todo App" /></a>
<br /><b>Vuejs Wisdom · Todo App, Composition 15 → 16</b>
<br />54 min · optional

</td>
<td valign="top">

**Watch:** [Vuejs Wisdom · Todo App, Composition 15 → 16](https://www.youtube.com/watch?v=QSBs0ceChnI&list=PLzjSlWqF2aTcUoouMnE9BTCvSxfrmcaQC&index=15) · **54 min · optional**

**Goal:** know the ways to style Vue, and use a component library wisely.

**Topics:** scoped styles & `lang` · CSS Modules in Vue · **Tailwind** with Vue · what component libraries are and when to use one · **PrimeVue**, **shadcn-vue**, **Nuxt UI** · icons · `<Teleport>`

**Watch:** [Scoped & lang, Options course 24](https://www.youtube.com/watch?v=FDUmao2ENkU&list=PLzjSlWqF2aTdehPN-zFc1TKcH8eNVn1JV&index=24) · 6 min

**Read:** [Tailwind with Vite](https://tailwindcss.com/docs/installation/using-vite) (same as week 7) · [shadcn-vue](https://www.shadcn-vue.com/) or [PrimeVue](https://primevue.org/): pick one, read its intro & install

</td>
</tr>
</table>

#### Task · Mini UI kit

A "**Component Gallery**" page with **Tailwind** + your chosen library:

- `BaseButton` (variants, sizes, loading) · `BaseInput` with label, error, `v-model` · `BaseCard` with header / default / footer slots · `BaseModal` (`<Teleport>`) · `Toast` · `Tabs` · `Dropdown Menu`
- All support **dark mode**
- Then swap them into your movies app

> [!TIP]
> **Bonus:** a `useToast()` composable: `toast.success("Saved")` from any component.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know what `scoped` does under the hood
- [ ] I know what problem `<Teleport>` solves
- [ ] I know a library like PrimeVue vs shadcn-vue, which copies code into your project
- [ ] My components work with the keyboard (Tab, Enter, Escape)

</details>

> [!WARNING]
> **Pitfalls:** several component libraries in one project · a library you can't customize.

> [!NOTE]
> **Mentor tip:** at work you'll rarely build a modal or dropdown from scratch (their accessibility is hard). But build one once, so you know what the library does for you.

<div align="right"><a href="#week-22">← Week 22</a> · <a href="#top">Top ↑</a> · <a href="#week-24">Week 24 →</a></div>

---

<a id="week-24"></a>

## Week 24 · Pinia

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=0e4D2ZJRe1E&list=PLfDx4cQoUNOZgZ5Lee5Lbj6jXlmCcupsm&index=1"><img src="https://img.youtube.com/vi/0e4D2ZJRe1E/mqdefault.jpg" width="320" alt="Pinia tutorial in Arabic" /></a>
<br /><b>Algorithm Academy · Pinia 1 → 7</b>
<br />50 min

</td>
<td valign="top">

**Watch:** [Algorithm Academy · Pinia 1 → 7](https://www.youtube.com/watch?v=0e4D2ZJRe1E&list=PLfDx4cQoUNOZgZ5Lee5Lbj6jXlmCcupsm&index=1) · **50 min**

**Goal:** manage shared state in a large app with Vue's official store.

**Topics:** when props and provide / inject aren't enough · what a store is · `defineStore`: state, getters, actions · **setup stores** (Composition style) · `storeToRefs` · Pinia DevTools · client vs server state

**Read:** **[Pinia intro](https://pinia.vuejs.org/introduction.html)** (short; see the setup store example) · [Core concepts](https://pinia.vuejs.org/core-concepts/)

</td>
</tr>
</table>

> [!NOTE]
> The course uses **options stores** (`state`, `getters`, `actions`). Try them, then rewrite the same store as a **setup store** (`ref`, `computed`, functions); it matches everything else you've learned.

#### Task · Shopping cart

A small store on [DummyJSON products](https://dummyjson.com/):

- Products, product details, and cart pages
- **`useCartStore`:** add, remove, quantity, total (getter), coupon discount
- **`useUiStore`:** sidebar open/closed, theme
- Cart persists in Local Storage
- Cart icon in the navbar shows the item count

> [!TIP]
> **Bonus:** a small Pinia plugin that persists any store to Local Storage automatically.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know when I need Pinia and when I don't
- [ ] I know options stores vs setup stores
- [ ] I know why `storeToRefs` is needed for destructuring state
- [ ] I can watch the store change in Vue DevTools

</details>

> [!WARNING]
> **Pitfalls:** everything in Pinia (form input state belongs in a component `ref`) · `const { count } = useStore()` without `storeToRefs` · API data in Pinia. That's **server state**: next week.

> [!NOTE]
> **Mentor tip:** Pinia is Vue's official store and replaced Vuex. A course or project using Vuex is outdated.

<div align="right"><a href="#week-23">← Week 23</a> · <a href="#top">Top ↑</a> · <a href="#week-25">Week 25 →</a></div>

---

<a id="week-25"></a>

## Week 25 · TanStack Query

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=KIS-MJfuPDY&list=PLejc1JbD4ZFRubkv6hV2D3r3eDoXTGHcF&index=1"><img src="https://img.youtube.com/vi/KIS-MJfuPDY/mqdefault.jpg" width="320" alt="TanStack Query concepts in Arabic" /></a>
<br /><b>kimz codes · TanStack Query concepts 1 → 19</b>
<br />2 h

</td>
<td valign="top">

**Watch:** [kimz codes · TanStack Query concepts 1 → 19](https://www.youtube.com/watch?v=KIS-MJfuPDY&list=PLejc1JbD4ZFRubkv6hV2D3r3eDoXTGHcF&index=1) · **2 h**

**Goal:** handle server data professionally: caching, refetching, mutations.

**Topics:** server vs client state · why `onMounted` + `fetch` doesn't scale · `useQuery`, query keys, `staleTime`, caching · DevTools · dependent & enabled queries · pagination · **`useMutation`** & invalidation · optimistic updates

**Main read:** **[TanStack Query for Vue](https://tanstack.com/query/latest/docs/framework/vue/overview)**: Overview, Quick Start, Queries, Mutations, Query Invalidation

</td>
</tr>
</table>

> [!NOTE]
> There's no Arabic course for Vue Query specifically. The Arabic course is in **React**, but **the concepts are identical** (keys, `staleTime`, caching, mutations, invalidation) and the API is nearly the same (`useQuery({ queryKey, queryFn })`). Watch for concepts, write Vue from the docs.

#### Task · Admin dashboard

Manage products or posts on [DummyJSON](https://dummyjson.com/):

- A table with **pagination** and search
- A details page per item
- **Add, edit, delete** with `useMutation`
- The table refreshes after changes (`invalidateQueries`)
- Skeleton loading instead of spinners
- **Not one `onMounted` fetch** in the whole project

> [!TIP]
> **Bonus:** **optimistic delete**: the row disappears instantly and comes back with an error if the request fails.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know server state vs client state
- [ ] I know `staleTime` vs `gcTime`
- [ ] I can make a query refetch when a `ref` changes (reactive query key)
- [ ] I can run a mutation and refresh data after it

</details>

> [!WARNING]
> **Pitfalls:** putting `page.value` in the key instead of the `ref` (or a getter), so the query never updates · copying query data into another `ref`.

> [!NOTE]
> **Mentor tip:** after TanStack Query you won't write fetches in `onMounted` again. It shows in code review.

<div align="right"><a href="#week-24">← Week 24</a> · <a href="#top">Top ↑</a> · <a href="#week-26">Week 26 →</a></div>

---

<a id="week-26"></a>

## Week 26 · Testing

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=hDZjJPPsWJw&list=PLDQ11FgmbqQOFLSRv-Ya39CchDjP1BLju&index=2"><img src="https://img.youtube.com/vi/hDZjJPPsWJw/mqdefault.jpg" width="320" alt="Testing concepts in Arabic" /></a>
<br /><b>Index Academy · Testing concepts 01 → 05</b>
<br />41 min

</td>
<td valign="top">

**Watch:** [Index Academy · Testing concepts 01 → 05](https://www.youtube.com/watch?v=hDZjJPPsWJw&list=PLDQ11FgmbqQOFLSRv-Ya39CchDjP1BLju&index=2) · **41 min**

**Goal:** write tests that prove your code works and catch what breaks when you change it later.

**Topics:** why test · unit, integration, E2E · **Vitest**: `describe`, `it`, `expect`, matchers · **Vue Test Utils** & **Testing Library for Vue** · testing Pinia stores · async tests · mocking

**Start here:** **[Testing · vuejs.org](https://vuejs.org/guide/scaling-up/testing.html)** (the whole picture)

**Read:** [Vitest guide](https://vitest.dev/guide/) · [Vue Test Utils](https://test-utils.vuejs.org/guide/) · [Vue Testing Library](https://testing-library.com/docs/vue-testing-library/intro) · [Playwright](https://playwright.dev/docs/intro) (for the bonus)

</td>
</tr>
</table>

> [!NOTE]
> The Arabic videos use React and Jest, but the first five cover **testing concepts** that apply everywhere. Vitest code looks almost exactly like Jest.

#### Task · Test the cart

On your week 24 shopping cart:

- **Unit tests** for the cart store: add, remove, quantity, total, coupon (5+, use `setActivePinia(createPinia())`)
- **Unit tests** for utilities (e.g. price formatting)
- **Component tests:** `ProductCard` shows name and price and "Add to Cart" emits or calls the store · `CartPage` shows an empty state and the correct total
- At least one test with a **mocked API**
- `npm run test:unit` all green

**Submit** the repo and a screenshot of the test results.

> [!TIP]
> **Bonus:** one **Playwright E2E test**: open the site, add a product, open the cart, check it's there.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know unit vs integration vs E2E
- [ ] I can test a Pinia store on its own
- [ ] I can assert that a component emitted an event
- [ ] I can mock a function and assert it was called
- [ ] My tests check **what users see**, not implementation details

</details>

> [!WARNING]
> **Pitfalls:** testing implementation (internal ref names) · tests that always pass. Break the code on purpose: does the test fail?

> [!NOTE]
> **Mentor tip:** you don't need 100% coverage. Start with what would hurt most if it broke: calculations, cart, auth.

<div align="right"><a href="#week-25">← Week 25</a> · <a href="#top">Top ↑</a> · <a href="#week-27">Week 27 →</a></div>

---

<a id="week-27"></a>

## Week 27 · Performance & Accessibility

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=lVpbayS9UUM&list=PLNknCqb-phEjLVnCbtVTJnWYml0zRvt5Y&index=1"><img src="https://img.youtube.com/vi/lVpbayS9UUM/mqdefault.jpg" width="320" alt="Web Accessibility 101" /></a>
<br /><b>Ahmed Saber · Web Accessibility 101</b>
<br />2.5 h

</td>
<td valign="top">

**Watch:** [Ahmed Saber · Web Accessibility 101](https://www.youtube.com/watch?v=lVpbayS9UUM&list=PLNknCqb-phEjLVnCbtVTJnWYml0zRvt5Y&index=1) · **2.5 h**

**Goal:** make your app fast, and usable by everyone.

**Performance:** how Vue tracks changes & re-renders · Vue DevTools performance · `v-once`, `v-memo`, `shallowRef` · computed vs method · lazy routes & `defineAsyncComponent` · Core Web Vitals (LCP, INP, CLS) · Lighthouse · images & bundle size

**Accessibility:** semantic HTML in Vue · keyboard & focus management (especially on route change) · ARIA (and when **not** to use it) · contrast · screen readers

**Read:** [Performance · vuejs.org](https://vuejs.org/guide/best-practices/performance.html) · [Accessibility · vuejs.org](https://vuejs.org/guide/best-practices/accessibility.html) · [Learn Performance](https://web.dev/learn/performance) · [Web Vitals](https://web.dev/articles/vitals) · [Learn Accessibility](https://web.dev/learn/accessibility)

**Tools:** [Lighthouse](https://developer.chrome.com/docs/lighthouse/overview) · [WAVE](https://wave.webaim.org/)

</td>
</tr>
</table>

#### Task · Audit & improve

On your biggest project from this level:

1. Run **Lighthouse** (mobile) and save a **before** screenshot
2. Use **Vue DevTools** to find components rendering too often
3. Lazy-load pages
4. Optimize images
5. **a11y:** use the app keyboard-only and fix what breaks; run WAVE and fix its errors
6. Save an **after** screenshot
7. In the README, a table: **problem → fix → before / after**

> [!TIP]
> **Bonus:** use your app with a **screen reader** (NVDA, VoiceOver, or TalkBack) for 5 minutes with your eyes closed. Write down how it felt.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know how Vue decides a component needs to update
- [ ] I know when `shallowRef` helps (big data you won't mutate deeply)
- [ ] I know what LCP, INP, and CLS mean
- [ ] I can read a Lighthouse report and know where to start
- [ ] My app works fully with the keyboard
- [ ] I know "**no ARIA is better than bad ARIA**"

</details>

> [!WARNING]
> **Pitfalls:** optimizing without measuring · `<div @click>` instead of `<button>`.

> [!NOTE]
> **Mentor tip:** **measure before you optimize.** Most beginner performance problems are huge images and code that loads before it's needed, not the framework.

<div align="right"><a href="#week-26">← Week 26</a> · <a href="#top">Top ↑</a> · <a href="#week-28">Week 28 →</a></div>

---

<a id="week-28"></a>

## Week 28 · Nuxt: Basics & Routing

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=q3T_NLWcZBo&list=PLzjSlWqF2aTcdEs97QvAU13E07llvv3UO&index=1"><img src="https://img.youtube.com/vi/q3T_NLWcZBo/mqdefault.jpg" width="320" alt="Learn Nuxt 3 in Arabic" /></a>
<br /><b>Vuejs Wisdom · Nuxt 3, 1 → 6</b>
<br />46 min

</td>
<td valign="top">

**Watch:** [Vuejs Wisdom · Nuxt 3, 1 → 6](https://www.youtube.com/watch?v=q3T_NLWcZBo&list=PLzjSlWqF2aTcdEs97QvAU13E07llvv3UO&index=1) · **46 min**

**Goal:** understand what Nuxt adds to Vue and build pages with file-based routing.

**Topics:** what a meta-framework is · CSR vs SSR vs SSG · setup & directory structure · **pages & routes** · dynamic routes · **layouts** & components · auto-imports · `NuxtLink` · assets

**Read:** [Nuxt intro](https://nuxt.com/docs/getting-started/introduction), then Installation, Directory Structure, Routing

</td>
</tr>
</table>

> [!NOTE]
> The course uses Nuxt 3; current is **Nuxt 4**. The main difference: app code now lives in `app/` (`app/pages/` instead of `pages/`). Most else is the same. When something differs, trust the docs.

#### Task · A blog in Nuxt

Start a blog (you'll finish it next week):

- `/` latest posts · `/blog` all posts · `/blog/[slug]` a post · `/about`
- A `default` layout with navbar and footer, a `blog` layout with a sidebar
- Posts in `data.ts` for now
- TypeScript + Tailwind

> [!TIP]
> **Bonus:** write posts as **Markdown** with [Nuxt Content](https://content.nuxt.com/).

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know CSR vs SSR vs SSG and when each fits
- [ ] I know how files become routes in Nuxt
- [ ] I know what auto-imports are and why I don't import `ref` or components
- [ ] I can build a dynamic route and read its params

</details>

> [!WARNING]
> **Pitfalls:** setting up `vue-router` by hand (Nuxt does it from `pages`) · touching `window` or `localStorage` anywhere. Code runs on the server first; use them inside `onMounted` or `<ClientOnly>`.

> [!NOTE]
> **Mentor tip:** Nuxt feels like magic at first (auto-imports and more). Read Directory Structure in the docs and you'll see where everything comes from.

<div align="right"><a href="#week-27">← Week 27</a> · <a href="#top">Top ↑</a> · <a href="#week-29">Week 29 →</a></div>

---

<a id="week-29"></a>

## Week 29 · Nuxt: Data, SEO & Deploy + AI Workflow

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=20WedKm6mcM&list=PLzjSlWqF2aTcdEs97QvAU13E07llvv3UO&index=7"><img src="https://img.youtube.com/vi/20WedKm6mcM/mqdefault.jpg" width="320" alt="Learn Nuxt 3 in Arabic part 2" /></a>
<br /><b>Vuejs Wisdom · Nuxt 3, 7 → 13</b>
<br />1 h

</td>
<td valign="top">

**Watch:** [Vuejs Wisdom · Nuxt 3, 7 → 13](https://www.youtube.com/watch?v=20WedKm6mcM&list=PLzjSlWqF2aTcdEs97QvAU13E07llvv3UO&index=7) · **1 h**

**Goal:** finish the blog with real data and SEO, ship it, and learn to use AI as a real work tool.

**Nuxt:** **`useFetch` & `useAsyncData`** · server routes (`server/api/`) · **SEO & meta** (`useSeoMeta`, `useHead`) · transitions · plugins & modules · error page · **middleware** · `useCookie` & `useState` · deploy

**AI workflow:** prompts with context, constraints, and a precise ask · AI for boilerplate, tests, explanations, reviews · **reviewing AI code**: never accept what you don't understand · common AI failures: outdated APIs (Vue 2, Options API, Nuxt 2), packages that don't exist, overcomplicated solutions

**Read:** [Nuxt docs](https://nuxt.com/docs/getting-started/introduction): Data Fetching, SEO and Meta, Deployment · [GitHub Copilot docs](https://docs.github.com/en/copilot)

</td>
</tr>
</table>

#### Task · Ship the blog

- Posts from an API (e.g. [DummyJSON posts](https://dummyjson.com/)) with `useFetch`
- At least one server route (`server/api/...`)
- **SEO:** `useSeoMeta` on every page; dynamic meta on posts
- A custom `error.vue`
- `/dashboard` protected by **route middleware**
- Page transitions
- **Deployed** on Vercel or Netlify, Lighthouse SEO & Performance **90+**

**AI task:** use any AI tool to (1) write tests for one component, (2) review one of your files, (3) explain a Nuxt concept you didn't get. In `AI_LOG.md`, record the exact prompt, the answer, and **what was wrong or needed fixing**.

**Submit** the repo, live link, and `AI_LOG.md`.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know `useFetch` vs `$fetch`, and why bare `$fetch` in setup can request twice
- [ ] I know where code runs: server, client, or both
- [ ] I can write a server route
- [ ] I can generate dynamic SEO meta
- [ ] I deployed a Nuxt app
- [ ] I can review AI-written code and catch its mistakes

</details>

> [!WARNING]
> **Pitfalls:** `$fetch` in setup instead of `useFetch` (one request on the server, another on the client) · asking AI to "build me a Nuxt blog" with no context gets you Nuxt 2 or the Options API. Give it the version, the API style, the file, and the exact ask.

> [!NOTE]
> **Mentor tip:** AI won't take your job. A developer who uses AI *well* might. The difference is catching its mistakes, which takes the fundamentals you spent 28 weeks building.

<div align="right"><a href="#week-28">← Week 28</a> · <a href="#top">Top ↑</a> · <a href="#week-30">Week 30 →</a></div>

---

<a id="week-30"></a>

## Week 30 · Graduation Project

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:059669,50:6366F1,100:A855F7&height=100&text=Graduation%20Project&fontSize=38&fontColor=ffffff&animation=twinkling" width="100%" alt="Graduation Project" />

</div>

**Goal:** build the strongest piece in your portfolio.

| Idea | Scope |
| :-- | :-- |
| **E-commerce** | Products, filters, search, cart, mock checkout, orders |
| **Admin dashboard** | Charts, sortable / filterable / paginated tables, full CRUD, dark mode |
| **Learning platform** | Courses, lessons, progress tracking, quizzes |
| **Job board** | Jobs, filters, company pages, saved jobs, applications |
| **CIS event platform** | Events, registration, QR tickets, admin panel |
| **Your idea** | Pitch it to your mentor first |

| Requirement | Details |
| :-- | :-- |
| **Stack** | **Nuxt** or **Vue + Vite**, TypeScript, Tailwind |
| **Pages** | 5+, including dynamic routes |
| **State** | Pinia for client state; TanStack Query (or `useFetch` in Nuxt) for server state |
| **Auth** | Login & register (mock or DummyJSON), protected routes |
| **Forms** | At least one complex validated form |
| **Testing** | 10+ tests (unit + component) |
| **Performance** | Lighthouse **90+** in all four |
| **Accessibility** | Fully keyboard-usable |
| **Responsive** | Mobile first |
| **Git** | Branches, PRs, clear commits |
| **Deploy** | Live on Vercel or Netlify |
| **README** | Screenshots or GIF, live link, stack & why, setup, challenges, what's next |

**Submit** the repo, live link, and a **2-3 minute demo video**.

<details>
<summary><b>Final exit checklist</b></summary>

<br />

- [ ] I can build a full Vue or Nuxt app from scratch on my own
- [ ] TypeScript feels natural
- [ ] I pick the right tool for each problem (state, fetching, styling)
- [ ] I test what matters
- [ ] I think about performance and accessibility from the start
- [ ] My GitHub has 3+ big, live projects with proper READMEs
- [ ] I use AI as a tool and catch its mistakes

</details>

> [!NOTE]
> **Mentor tip:** one **finished, polished** project beats ten tutorial clones. Interviewers will open it and ask "why did you do it this way?" everywhere. Know every answer.

<div align="right"><a href="#week-29">← Week 29</a> · <a href="#top">Top ↑</a></div>

---

<div align="center">

## You finished the roadmap.

You did what most people who start quit halfway through.

</div>

| Next | |
| :-- | :-- |
| **Portfolio** | Build a personal site in Nuxt showing your projects |
| **Open source** | Vue and Nuxt communities welcome newcomers; look for `good first issue` |
| **Some backend** | Nuxt server routes with a database, or Laravel (a classic pair with Vue) |
| **Apply** | Internships, even if you don't feel ready. You're more ready than you think. |
| **Teach** | Write about what you learned, or help someone in Level 1. Nothing teaches like explaining. |

<div align="center">

<a href="README.md"><img src="https://img.shields.io/badge/←_Back_to_the_Roadmap-6366F1?style=for-the-badge" alt="Back to the roadmap" /></a>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:34D399,100:059669&height=110&section=footer" width="100%" alt="" />

</div>
