<a id="top"></a>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0891B2,100:22D3EE&height=200&section=header&text=Level%203%20%C2%B7%20React&fontSize=56&fontColor=ffffff&fontAlignY=38&animation=fadeIn&desc=React%20%C2%B7%20Router%20%C2%B7%20State%20%C2%B7%20Testing%20%C2%B7%20Next.js&descSize=18&descAlignY=60" width="100%" alt="Level 3 React" />

<img src="https://skillicons.dev/icons?i=react,ts,redux,tailwind,vitest,nextjs,vercel" alt="React TypeScript Redux Tailwind Vitest Next.js Vercel" />

<br /><br />

<img src="https://img.shields.io/badge/Weeks-19_→_30-0891B2?style=for-the-badge" alt="Weeks 19-30" />
<img src="https://img.shields.io/badge/Video-~29_h-22D3EE?style=for-the-badge" alt="About 29 hours of video" />
<img src="https://img.shields.io/badge/React-19-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React 19" />
<img src="https://img.shields.io/badge/Next.js-App_Router-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js App Router" />

<br /><br />

[Roadmap](README.md) · [Beginner](01-beginner.md) · [Intermediate](02-intermediate.md) · **React** · [Vue](03-vue.md) · [Tracker](TRACKER.md)

</div>

---

Remember week 12, updating the UI by hand every time data changed? React says: **describe what the UI looks like for this data, and I'll handle the rest.**

You'll learn React, then the tools every real React project uses, and finish with **Next.js**, which turns React from a library into a full framework.

| Week | Topic | You ship |
| :--: | :-- | :-- |
| [19](#week-19) | Components, JSX, props | Landing page as components |
| [20](#week-20) | State, events, forms | A multi-step form |
| [21](#week-21) | Context, effects, data fetching | Movies app |
| [22](#week-22) | React Router | A multi-page app |
| [23](#week-23) | Styling & component libraries | A mini UI kit |
| [24](#week-24) | State management | A shopping cart |
| [25](#week-25) | TanStack Query | An admin dashboard |
| [26](#week-26) | Testing | Tests for the cart |
| [27](#week-27) | Performance & accessibility | An audit, before & after |
| [28](#week-28) | Next.js: basics & routing | A blog |
| [29](#week-29) | Next.js: data, SEO, deploy + AI workflow | The blog, live |
| [30](#week-30) | **Graduation project** | A complete app |

> [!IMPORTANT]
> **Main Arabic source:** [React course · Tarmeez Academy](https://www.youtube.com/playlist?list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS), 120+ lessons full of challenges with solutions. When something feels outdated, **[react.dev](https://react.dev/learn)** is the source of truth ([Arabic version](https://ar.react.dev/learn)).
>
> **From now on, every React project is TypeScript.** Courses are mostly JS: watch in JS, write in TS. Stuck? [React + TypeScript](https://react.dev/learn/typescript).

---

<a id="week-19"></a>

## Week 19 · Components, JSX & Props

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=T9DTxrQ1BU0&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=3"><img src="https://img.youtube.com/vi/T9DTxrQ1BU0/mqdefault.jpg" width="320" alt="Tarmeez React lesson 1" /></a>
<br /><b>Tarmeez · React lessons 1 → 20</b>
<br />4 h

</td>
<td valign="top">

**Watch:** [Tarmeez · React lessons 1 → 20](https://www.youtube.com/watch?v=T9DTxrQ1BU0&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=3) · **4 h**

**Goal:** think in React: everything is a component, and components talk through props.

**Topics:** why React · new project with Vite (`npm create vite@latest` → React + TS) · project structure · **components** & **JSX** · styles & classes in JSX · **props** & `children` · conditional rendering · lists & `key`

**Quick review:** [React basics in 90 min · Yehia Tech](https://www.youtube.com/playlist?list=PL8q8h6vqfkSVeuw14BwrtJRIg3tAwq0ds)

**Read:** [Quick Start](https://react.dev/learn) · **[Thinking in React](https://react.dev/learn/thinking-in-react)** (the key read this week)

</td>
</tr>
</table>

> [!NOTE]
> If the course uses `create-react-app`, **use Vite instead.** CRA is deprecated.

#### Task · Landing page as components

Rebuild your week 8 landing page in React + TypeScript:

- Split it up: `Navbar`, `Hero`, `Features`, `FeatureCard`, `Testimonials`, `Footer`...
- Anything repeated (cards, testimonials, nav links) becomes an **array of objects** rendered with `map`
- Every component has a clear `Props` type
- No component much longer than ~80 lines

> [!TIP]
> **Bonus:** a `Button` with `variant` (`"primary" | "secondary" | "ghost"`) and `size` (`"sm" | "md" | "lg"`), used across the page.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know how JSX differs from HTML (`className`, `htmlFor`, `{}`, self-closing)
- [ ] I know why `key` matters and why the index isn't always OK
- [ ] I know props are **read-only**
- [ ] I can look at a design and see the components
- [ ] I know what `children` is for

</details>

> [!WARNING]
> **Pitfalls:** one giant `App` component · a missing `key`, or `Math.random()` as the key · defining a component inside another component.

> [!NOTE]
> **Mentor tip:** read *Thinking in React* twice. That page alone separates people who write React from people who understand it.

<div align="right"><a href="#top">Top ↑</a> · <a href="#week-20">Week 20 →</a></div>

---

<a id="week-20"></a>

## Week 20 · State, Events & Forms

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=rnVI3UKcKQA&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=25"><img src="https://img.youtube.com/vi/rnVI3UKcKQA/mqdefault.jpg" width="320" alt="Tarmeez React lesson 21" /></a>
<br /><b>Tarmeez · React lessons 21 → 40</b>
<br />3.5 h

</td>
<td valign="top">

**Watch:** [Tarmeez · React lessons 21 → 40](https://www.youtube.com/watch?v=rnVI3UKcKQA&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=25) · **3.5 h**

**Goal:** make components remember things and react to the user.

**Topics:** why a normal variable isn't enough · how React re-renders · **`useState`** · events & handlers · **forms**: controlled inputs, select, radio, checkbox · **immutability** for objects & arrays · updater functions `setCount(c => c + 1)`

**Optional build:** [Tarmeez · Loan Application Form project, lessons 41 → 43](https://www.youtube.com/watch?v=hFrOluMFZxA&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=45) · 1.5 h

**Read:** [Adding Interactivity](https://react.dev/learn/adding-interactivity) · [Managing State](https://react.dev/learn/managing-state)

</td>
</tr>
</table>

> [!TIP]
> Tarmeez has **a challenge after each part, then a solution video.** Solve it first. If you got it right, watch the solution at 1.5x.

#### Task · Multi-step form

A 3-step course application form:

1. **Personal:** name, email, phone
2. **Academic:** college, year, track (radio), skills (checkboxes)
3. **Review:** all data + submit

- A progress bar for the current step
- **Validation** per step before moving on, errors under each input
- Going back keeps the data
- **One** state object for the whole form, updated **immutably**
- After submit: success message, form resets

> [!TIP]
> **Bonus:** save the form to Local Storage as the user types, so closing the tab by accident loses nothing.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know why `count = count + 1` changes nothing on screen
- [ ] I know why `state.push(item)` is wrong and what to do instead
- [ ] I know state updates aren't instant (batching)
- [ ] I know when to use `prev => ...`
- [ ] I know controlled vs uncontrolled inputs

</details>

> [!WARNING]
> **Pitfalls:** state for things you can compute (`total` from `items`) · mutating state directly (`user.name = "x"`) · `onClick={handleClick()}`, which runs immediately.

> [!NOTE]
> **Mentor tip:** before `useState`, ask: "does this change? can I compute it from something I already have?" Half of beginner state isn't needed.

<div align="right"><a href="#week-19">← Week 19</a> · <a href="#top">Top ↑</a> · <a href="#week-21">Week 21 →</a></div>

---

<a id="week-21"></a>

## Week 21 · Context, Effects & Data Fetching

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=nalt9TkgOlE&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=48"><img src="https://img.youtube.com/vi/nalt9TkgOlE/mqdefault.jpg" width="320" alt="Tarmeez React lesson 44" /></a>
<br /><b>Tarmeez · React lessons 44 → 51</b>
<br />1.5 h

</td>
<td valign="top">

**Watch:** [Tarmeez · React lessons 44 → 51](https://www.youtube.com/watch?v=nalt9TkgOlE&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=48) · **1.5 h**

**Goal:** share data between distant components and load data from an API.

**Topics:** lifting state up · prop drilling · **`useContext`** · **`useEffect`**: timing, dependencies, **cleanup** · API requests · loading & error states · i18n and switching RTL / LTR

**Also watch:** [Tarmeez · API & useEffect, weather project, lessons 97 → 109](https://www.youtube.com/watch?v=EJ7-xQ1l5-c&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=102) · 2.5 h

**Read:** [Synchronizing with Effects](https://react.dev/learn/synchronizing-with-effects) · **[You Might Not Need an Effect](https://react.dev/learn/you-might-not-need-an-effect)** (saves you many bugs)

</td>
</tr>
</table>

#### Task · Movies app

If your Project 2 was a movies app, rebuild it in React. Otherwise build one now with [TMDB](https://www.themoviedb.org/documentation/api) or [DummyJSON](https://dummyjson.com/):

- A list from the API with debounced search
- A **custom hook** `useFetch<T>(url)` returning `{ data, isLoading, error }`
- **ThemeContext** for dark mode
- **FavoritesContext**, persisted in Local Storage
- Proper cleanup: fast typing never shows a stale result (`AbortController`)

> [!TIP]
> **Bonus:** an Arabic / English toggle that flips the page between RTL and LTR, like Tarmeez's weather project.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know `useEffect(fn)` vs `useEffect(fn, [])` vs `useEffect(fn, [x])`
- [ ] I know when cleanup runs and why it matters
- [ ] I know why effects run twice in development (Strict Mode)
- [ ] I know when Context fits and when plain props are better
- [ ] I can write a custom hook

</details>

> [!WARNING]
> **Pitfalls:** an effect to compute derived values (just compute during render) · infinite loops (setting state that's in the deps) · Context for everything. It's a *delivery* mechanism, not state management, and every change re-renders all consumers.

> [!NOTE]
> **Mentor tip:** **an effect means syncing with something outside React** (API, timer, DOM, storage). Nothing outside React? You probably don't need one.

<div align="right"><a href="#week-20">← Week 20</a> · <a href="#top">Top ↑</a> · <a href="#week-22">Week 22 →</a></div>

---

<a id="week-22"></a>

## Week 22 · React Router

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=bkj8obp1XmA&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=55"><img src="https://img.youtube.com/vi/bkj8obp1XmA/mqdefault.jpg" width="320" alt="Tarmeez React lesson 52" /></a>
<br /><b>Tarmeez · React lessons 52 → 58</b>
<br />1.5 h

</td>
<td valign="top">

**Watch:** [Tarmeez · React lessons 52 → 58](https://www.youtube.com/watch?v=bkj8obp1XmA&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=55) · **1.5 h**

**Goal:** build a multi-page app with no full page reloads.

**Topics:** SPA · CSR vs SSR · routes, `Link`, `NavLink` · **dynamic routes** & `useParams` · 404 page · **nested routes**, layouts, `Outlet` · `useNavigate` & `useSearchParams` · protected routes

**Read:** [React Router docs](https://reactrouter.com/home) · [Declarative mode install](https://reactrouter.com/start/declarative/installation)

</td>
</tr>
</table>

> [!NOTE]
> React Router v7 has 3 modes. Use **Declarative mode**: it's closest to the course and simplest to start with.

#### Task · Multi-page app

Extend your movies app (or start fresh):

- `/` home · `/movies` list with search & filter **in the URL** (`?q=batman&genre=action`) · `/movies/:id` details · `/favorites`
- `/login` (fake login sets a user in Context) · `/profile` **protected**, redirects to `/login`
- A proper 404 page
- A shared layout with navbar and footer; `NavLink` highlights the current page

> [!IMPORTANT]
> Refresh on `/movies/5` after deploying gives a 404? Look up "SPA redirect rules" for Netlify or Vercel.

> [!TIP]
> **Bonus:** lazy-load each page with `React.lazy` + `Suspense`.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know `<a>` vs `<Link>`
- [ ] I know `useParams` vs `useSearchParams`
- [ ] I know why the URL can be better than `useState`
- [ ] I can build a protected route
- [ ] I know why SPAs 404 on refresh and how to fix it

</details>

> [!WARNING]
> **Pitfalls:** `<a href>` instead of `<Link>` (full reload, state lost) · forgetting `<Outlet />` in a layout.

> [!NOTE]
> **Mentor tip:** the URL is the web's oldest and best state manager. Anything a user might share (search, filters, page) belongs in it.

<div align="right"><a href="#week-21">← Week 21</a> · <a href="#top">Top ↑</a> · <a href="#week-23">Week 23 →</a></div>

---

<a id="week-23"></a>

## Week 23 · Styling & Component Libraries

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=T9iM1LVNKec&list=PLdnrjoDUmGZ8Q9Dq9ebR9v1xEgqJ6tcfx&index=11"><img src="https://img.youtube.com/vi/T9iM1LVNKec/mqdefault.jpg" width="320" alt="React 19 and Tailwind 4 landing page" /></a>
<br /><b>Triangles · React 19 + Tailwind 4 landing page → Vercel</b>
<br />1 h

</td>
<td valign="top">

**Watch:** [Triangles · React 19 + Tailwind 4 landing page → Vercel](https://www.youtube.com/watch?v=T9iM1LVNKec&list=PLdnrjoDUmGZ8Q9Dq9ebR9v1xEgqJ6tcfx&index=11) · **1 h**

**Goal:** know the ways to style React, and use a component library wisely.

**Topics:** plain CSS · CSS Modules · **Tailwind** in React & conditional classes (`clsx`) · what component libraries are and when to use one · **shadcn/ui** · Material UI · icons (`lucide-react`)

**Also watch:** [Tarmeez · Material UI, lessons 59 → 64](https://www.youtube.com/watch?v=qwtcYDWf1EU&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=62) · 57 min

**Optional build:** [Tarmeez · To-do project, lessons 65 → 84](https://www.youtube.com/watch?v=nRsXnEIyPog&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=68) · 4 h

**Read:** [shadcn/ui docs](https://ui.shadcn.com/docs): Introduction + Vite installation

</td>
</tr>
</table>

#### Task · Mini UI kit

A "**Component Gallery**" page built with **Tailwind + shadcn/ui**:

- `Button` (variants, sizes, loading) · `Input` with label and error · `Card` · `Modal` / `Dialog` · `Toast` · `Tabs` · `Dropdown Menu`
- All support **dark mode**
- Then swap them into your movies app

> [!TIP]
> **Bonus:** a full toast system on Context: `const { toast } = useToast()` → `toast.success("Saved")` from anywhere.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know a library like MUI vs shadcn/ui, which copies code into your project
- [ ] I can write conditional Tailwind classes cleanly
- [ ] I know when to use a library and when to build it myself
- [ ] My components work with the keyboard (Tab, Enter, Escape)

</details>

> [!WARNING]
> **Pitfalls:** three component libraries in one project · using a library you can't customize. If you can't change the button color, you don't control your app.

> [!NOTE]
> **Mentor tip:** at work you'll rarely build a modal or dropdown from scratch (their accessibility is hard). But build one once, so you know what the library is doing for you.

<div align="right"><a href="#week-22">← Week 22</a> · <a href="#top">Top ↑</a> · <a href="#week-24">Week 24 →</a></div>

---

<a id="week-24"></a>

## Week 24 · State Management

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=G3jSV8p9li0&list=PLxRKoQzM5m3J6gDMz-_eqLvxIR6UH0Pf7&index=1"><img src="https://img.youtube.com/vi/G3jSV8p9li0/mqdefault.jpg" width="320" alt="Redux Toolkit in Arabic" /></a>
<br /><b>Simple Arab Code · Redux Toolkit 1 → 13</b>
<br />2.5 h

</td>
<td valign="top">

**Watch:** [Simple Arab Code · Redux Toolkit 1 → 13](https://www.youtube.com/watch?v=G3jSV8p9li0&list=PLxRKoQzM5m3J6gDMz-_eqLvxIR6UH0Pf7&index=1) · **2.5 h**

**Goal:** manage complex, shared state in a large app.

**Topics:** when `useState` and Context aren't enough · **`useReducer`**, reducer + context · **Redux Toolkit**: store, slices, `useSelector`, `useDispatch`, async thunks, DevTools · **Zustand**, the lighter alternative · client vs server state

**Also watch:** [Tarmeez · useReducer, lessons 91 → 94](https://www.youtube.com/watch?v=_IOM9XtJAvE&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=95) · 2 h

**Alternative:** [Tarmeez · Redux, lessons 110 → 124](https://www.youtube.com/watch?v=7bPnRc_BDe8&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=115) · 3.5 h

**Read:** [Zustand intro](https://zustand.docs.pmnd.rs/learn/getting-started/introduction) (very short) · [Reducer + Context](https://react.dev/learn/scaling-up-with-reducer-and-context) · [RTK Quick Start](https://redux-toolkit.js.org/tutorials/quick-start)

</td>
</tr>
</table>

#### Task · Shopping cart

A small store on [DummyJSON products](https://dummyjson.com/):

- Products, product details, and cart pages
- **Cart in Redux Toolkit:** add, remove, change quantity, total, coupon discount
- **UI state in Zustand:** sidebar open/closed, theme
- Cart persists in Local Storage
- Cart icon in the navbar shows the item count

> [!TIP]
> **Bonus:** build the same cart in Zustand only. Compare line counts and readability, and write your verdict in the README.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know when I need a state library and when I don't
- [ ] I know `useState` vs `useReducer`
- [ ] I understand the Redux flow: action → reducer → store → UI
- [ ] I know why RTK lets me write `state.items.push()` (Immer)
- [ ] I know Redux vs Zustand

</details>

> [!WARNING]
> **Pitfalls:** everything in Redux (form input state belongs in `useState`) · API data in Redux. That's **server state**: next week.

> [!NOTE]
> **Mentor tip:** Redux Toolkit is still everywhere in Egyptian companies, so know it. In new projects, Zustand + TanStack Query cover most needs with far less code.

<div align="right"><a href="#week-23">← Week 23</a> · <a href="#top">Top ↑</a> · <a href="#week-25">Week 25 →</a></div>

---

<a id="week-25"></a>

## Week 25 · TanStack Query

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=KIS-MJfuPDY&list=PLejc1JbD4ZFRubkv6hV2D3r3eDoXTGHcF&index=1"><img src="https://img.youtube.com/vi/KIS-MJfuPDY/mqdefault.jpg" width="320" alt="TanStack Query in Arabic" /></a>
<br /><b>kimz codes · TanStack Query 1 → 19</b>
<br />2 h

</td>
<td valign="top">

**Watch:** [kimz codes · TanStack Query 1 → 19](https://www.youtube.com/watch?v=KIS-MJfuPDY&list=PLejc1JbD4ZFRubkv6hV2D3r3eDoXTGHcF&index=1) · **2 h**

**Goal:** handle server data professionally: caching, refetching, mutations.

**Topics:** server vs client state · why `useEffect` + `fetch` doesn't scale · `useQuery`, query keys, `staleTime`, caching · DevTools · dependent & enabled queries · pagination · prefetching · **`useMutation`** & invalidation · optimistic updates

**Continue:** [Optimistic updates, 20 → 22](https://www.youtube.com/watch?v=9M6A2tfis-g&list=PLejc1JbD4ZFRubkv6hV2D3r3eDoXTGHcF&index=20) · 28 min

**Read:** [TanStack Query overview](https://tanstack.com/query/latest/docs/framework/react/overview)

</td>
</tr>
</table>

#### Task · Admin dashboard

Manage products or posts on [DummyJSON](https://dummyjson.com/):

- A table with **pagination** and search
- A details page per item
- **Add, edit, delete** with `useMutation`
- The table refreshes after changes (`invalidateQueries`)
- Skeleton loading instead of spinners
- **Not one `useEffect` for fetching** in the whole project

> [!NOTE]
> DummyJSON simulates writes without saving them. Fine for practice: you'll see the change in the response.

> [!TIP]
> **Bonus:** **optimistic delete**: the row disappears instantly and comes back with an error if the request fails.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know server state vs client state
- [ ] I know `staleTime` vs `gcTime`
- [ ] I know why query keys include every variable (`['products', page, search]`)
- [ ] I can run a mutation and refresh data after it
- [ ] I use React Query DevTools and understand what it shows

</details>

> [!WARNING]
> **Pitfalls:** a static query key (`['products']`) while the page changes · copying query data into `useState`.

> [!NOTE]
> **Mentor tip:** after TanStack Query you won't go back to `useEffect` + `fetch`. It shows in code review.

<div align="right"><a href="#week-24">← Week 24</a> · <a href="#top">Top ↑</a> · <a href="#week-26">Week 26 →</a></div>

---

<a id="week-26"></a>

## Week 26 · Testing

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=hDZjJPPsWJw&list=PLDQ11FgmbqQOFLSRv-Ya39CchDjP1BLju&index=2"><img src="https://img.youtube.com/vi/hDZjJPPsWJw/mqdefault.jpg" width="320" alt="React Testing in Arabic" /></a>
<br /><b>Index Academy · React Testing 01 → 15</b>
<br />2.5 h

</td>
<td valign="top">

**Watch:** [Index Academy · React Testing 01 → 15](https://www.youtube.com/watch?v=hDZjJPPsWJw&list=PLDQ11FgmbqQOFLSRv-Ya39CchDjP1BLju&index=2) · **2.5 h**

**Goal:** write tests that prove your code works and catch what breaks when you change it later.

**Topics:** why test · unit, integration, E2E · **Vitest**: `describe`, `it`, `expect`, matchers · **React Testing Library**: `render`, `screen`, queries (`getByRole`...) · user events · async tests · mocking functions & API calls · intro to TDD

**Read:** [Vitest guide](https://vitest.dev/guide/) · [React Testing Library](https://testing-library.com/docs/react-testing-library/intro/) · [Playwright](https://playwright.dev/docs/intro) (for the bonus)

</td>
</tr>
</table>

> [!NOTE]
> The Arabic course uses **Jest**; we use **Vitest** because it works with Vite out of the box. The code is nearly identical (`describe`, `it`, `expect`); you write `vi.fn()` instead of `jest.fn()`.

#### Task · Test the cart

On your week 24 shopping cart:

- **Unit tests** for the slice: add, remove, quantity, total, coupon (5+ tests)
- **Unit tests** for utilities (e.g. price formatting)
- **Component tests:** `ProductCard` shows name and price and "Add to Cart" calls the handler · `CartPage` shows an empty state and the correct total
- At least one test with a **mocked API**
- `npm run test` all green

**Submit** the repo and a screenshot of the test results.

> [!TIP]
> **Bonus:** one **Playwright E2E test**: open the site, add a product, open the cart, check it's there.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know unit vs integration vs E2E
- [ ] I know why `getByRole` beats `getByTestId` in most cases
- [ ] I know `getBy` vs `queryBy` vs `findBy`
- [ ] I can mock a function and assert it was called
- [ ] My tests check **what users see**, not implementation details

</details>

> [!WARNING]
> **Pitfalls:** testing implementation (state names, render counts) · tests that always pass. Break the code on purpose: does the test fail?

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

**Performance:** what triggers a re-render · React DevTools Profiler · `memo`, `useMemo`, `useCallback`, and **when not to** · **React Compiler** (auto-memoization) · code splitting & `lazy` · Core Web Vitals (LCP, INP, CLS) · Lighthouse · images (lazy loading, sizing, WebP / AVIF) · bundle size

**Accessibility:** semantic HTML in React · keyboard & focus management · ARIA (and when **not** to use it) · color contrast · screen readers

**Also watch:** [Tarmeez · useMemo, lesson 86](https://www.youtube.com/watch?v=5xWJIRJDQXM&list=PLYyqC4bNbCIdSZ-JayMLl4WO2Cr995vyS&index=89) · 16 min

**Read:** [Learn Performance · web.dev](https://web.dev/learn/performance) · [memo](https://react.dev/reference/react/memo) · [useMemo](https://react.dev/reference/react/useMemo) · [lazy](https://react.dev/reference/react/lazy) · [React Compiler](https://react.dev/learn/react-compiler) · [Web Vitals](https://web.dev/articles/vitals) · [Learn Accessibility](https://web.dev/learn/accessibility)

**Tools:** [Lighthouse](https://developer.chrome.com/docs/lighthouse/overview) · [WAVE](https://wave.webaim.org/)

</td>
</tr>
</table>

#### Task · Audit & improve

On your biggest project from this level:

1. Run **Lighthouse** (mobile) and save a **before** screenshot
2. Use the **Profiler** to find pointless re-renders
3. Add **code splitting** for pages
4. Optimize images
5. **a11y:** use the app keyboard-only and fix what breaks; run WAVE and fix its errors
6. Save an **after** screenshot
7. In the README, a table: **problem → fix → before / after**

> [!TIP]
> **Bonus:** use your app with a **screen reader** (NVDA, VoiceOver, or TalkBack) for 5 minutes with your eyes closed. Write down how it felt.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know what makes a React component re-render
- [ ] I know when `useMemo` / `useCallback` help and when they hurt
- [ ] I know what LCP, INP, and CLS mean
- [ ] I can read a Lighthouse report and know where to start
- [ ] My app works fully with the keyboard
- [ ] I know "**no ARIA is better than bad ARIA**"

</details>

> [!WARNING]
> **Pitfalls:** `useMemo` on everything (memoization has a cost; measure first) · `<div onClick>` instead of `<button>` (no keyboard, invisible to screen readers).

> [!NOTE]
> **Mentor tip:** **measure before you optimize.** Most beginner performance problems are huge images and code that loads before it's needed, not re-renders.

<div align="right"><a href="#week-26">← Week 26</a> · <a href="#top">Top ↑</a> · <a href="#week-28">Week 28 →</a></div>

---

<a id="week-28"></a>

## Week 28 · Next.js: Basics & Routing

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=P6n44p4k9U8&list=PLSDhifuM5C420tyw98jx-ZesncZVtOyPB&index=1"><img src="https://img.youtube.com/vi/P6n44p4k9U8/mqdefault.jpg" width="320" alt="Next.js course 2026" /></a>
<br /><b>Saad Al-Sattouf · Next.js 2026, 1 → 12</b>
<br />1.5 h

</td>
<td valign="top">

**Watch:** [Saad Al-Sattouf · Next.js 2026, 1 → 12](https://www.youtube.com/watch?v=P6n44p4k9U8&list=PLSDhifuM5C420tyw98jx-ZesncZVtOyPB&index=1) · **1.5 h**

**Goal:** understand what Next.js adds to React and build pages with the App Router.

**Topics:** what a meta-framework is · CSR vs SSR vs SSG · project setup & file structure · **App Router**, folder-based routing · `Link` · dynamic & nested routes · **layouts** & nested layouts · route params

**Course:** **[Learn Next.js](https://nextjs.org/learn)** (official, interactive, free)

**Read:** [Next.js docs](https://nextjs.org/docs)

</td>
</tr>
</table>

#### Task · A blog in Next.js

Start a blog (you'll finish it next week):

- `/` latest posts · `/blog` all posts · `/blog/[slug]` a post · `/about`
- A root layout with navbar and footer, and a blog layout with a sidebar
- Posts in `data.ts` for now
- TypeScript + Tailwind

> [!TIP]
> **Bonus:** write posts as **Markdown** files and render them (see MDX in the Next.js docs).

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know CSR vs SSR vs SSG and when each fits
- [ ] I know how folders become routes in the App Router
- [ ] I know `page.tsx` vs `layout.tsx`
- [ ] I can build a dynamic route and read its params

</details>

> [!WARNING]
> **Pitfalls:** following a **Pages Router** (`pages/`) tutorial. We use the **App Router** (`app/`) · `"use client"` at the top of every file (more on that next week).

> [!NOTE]
> **Mentor tip:** Next.js feels like relearning React at first. It isn't. Everything you know still works; Next.js adds *where* things render: server or client.

<div align="right"><a href="#week-27">← Week 27</a> · <a href="#top">Top ↑</a> · <a href="#week-29">Week 29 →</a></div>

---

<a id="week-29"></a>

## Week 29 · Next.js: Data, SEO & Deploy + AI Workflow

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=cTNbmYbEa9w&list=PLSDhifuM5C420tyw98jx-ZesncZVtOyPB&index=13"><img src="https://img.youtube.com/vi/cTNbmYbEa9w/mqdefault.jpg" width="320" alt="Next.js course 2026 part 2" /></a>
<br /><b>Saad Al-Sattouf · Next.js 2026, 13 → 20</b>
<br />1 h

</td>
<td valign="top">

**Watch:** [Saad Al-Sattouf · Next.js 2026, 13 → 20](https://www.youtube.com/watch?v=cTNbmYbEa9w&list=PLSDhifuM5C420tyw98jx-ZesncZVtOyPB&index=13) · **1 h**

**Goal:** finish the blog with real data and SEO, ship it, and learn to use AI as a real work tool.

**Next.js:** **Server vs Client Components** & `"use client"` · fetching in Server Components · route handlers · `loading.tsx`, `error.tsx`, `not-found.tsx` · **metadata & SEO** · `next/image` & `next/font` · deploy on Vercel

**AI workflow:** prompts with context, constraints, and a precise ask · AI for boilerplate, tests, explanations, reviews · **reviewing AI code**: never accept what you don't understand · common AI failures: outdated APIs, packages that don't exist, overcomplicated solutions

**Optional:** [Level 2: auth, middleware, deploy, 21 → 30](https://www.youtube.com/watch?v=ZzDG94HAEgM&list=PLSDhifuM5C420tyw98jx-ZesncZVtOyPB&index=21) · 2 h

**Read:** [Learn Next.js](https://nextjs.org/learn) · [GitHub Copilot docs](https://docs.github.com/en/copilot)

</td>
</tr>
</table>

#### Task · Ship the blog

- Posts from an API (e.g. [DummyJSON posts](https://dummyjson.com/)) in a **Server Component**
- Like button and comment form as **Client Components** (the only `"use client"` files)
- At least one route handler (`/api/...`)
- `loading.tsx` with skeletons, `error.tsx`, `not-found.tsx`
- **Metadata** on every page; dynamic metadata on posts
- `next/image` for all images, `next/font` for fonts
- **Deployed on Vercel**, Lighthouse SEO & Performance **90+**

**AI task:** use any AI tool to (1) write tests for one component, (2) review one of your files, (3) explain a Next.js concept you didn't get. In `AI_LOG.md`, record the exact prompt, the answer, and **what was wrong or needed fixing**.

**Submit** the repo, live link, and `AI_LOG.md`.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know Server vs Client Components and when I need `"use client"`
- [ ] I know why `useState` can't be used in a Server Component
- [ ] I can fetch data in a Server Component without `useEffect`
- [ ] I can generate dynamic metadata
- [ ] I deployed a Next.js app on Vercel
- [ ] I can review AI-written code and catch its mistakes

</details>

> [!WARNING]
> **Pitfalls:** `"use client"` in the root layout makes the whole app client-side · asking AI to "build me a Next.js blog" with no context gets you old versions or the Pages Router. Give it the version, the router, the file, and the exact ask.

> [!NOTE]
> **Mentor tip:** AI won't take your job. A developer who uses AI *well* might. The difference is catching its mistakes, which takes the fundamentals you spent 28 weeks building.

<div align="right"><a href="#week-28">← Week 28</a> · <a href="#top">Top ↑</a> · <a href="#week-30">Week 30 →</a></div>

---

<a id="week-30"></a>

## Week 30 · Graduation Project

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0891B2,50:6366F1,100:A855F7&height=100&text=Graduation%20Project&fontSize=38&fontColor=ffffff&animation=twinkling" width="100%" alt="Graduation Project" />

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
| **Stack** | **Next.js** (App Router) or **React + Vite**, TypeScript `strict`, Tailwind |
| **Pages** | 5+, including dynamic routes |
| **State** | Zustand or RTK for client state; TanStack Query or Server Components for server state |
| **Auth** | Login & register (mock or DummyJSON), protected routes |
| **Forms** | At least one complex validated form |
| **Testing** | 10+ tests (unit + component) |
| **Performance** | Lighthouse **90+** in all four |
| **Accessibility** | Fully keyboard-usable |
| **Responsive** | Mobile first |
| **Git** | Branches, PRs, clear commits |
| **Deploy** | Live on Vercel |
| **README** | Screenshots or GIF, live link, stack & why, setup, challenges, what's next |

**Submit** the repo, live link, and a **2-3 minute demo video**.

<details>
<summary><b>Final exit checklist</b></summary>

<br />

- [ ] I can build a full React or Next.js app from scratch on my own
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
| **Portfolio** | Build a personal site in Next.js showing your projects |
| **Open source** | Look for `good first issue` in projects you use |
| **Some backend** | Node.js + Express, or Next.js route handlers with a database |
| **Apply** | Internships, even if you don't feel ready. You're more ready than you think. |
| **Teach** | Write about what you learned, or help someone in Level 1. Nothing teaches like explaining. |

<div align="center">

<a href="README.md"><img src="https://img.shields.io/badge/←_Back_to_the_Roadmap-6366F1?style=for-the-badge" alt="Back to the roadmap" /></a>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:22D3EE,100:0891B2&height=110&section=footer" width="100%" alt="" />

</div>
