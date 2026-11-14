<a id="top"></a>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:EA580C,100:F59E0B&height=200&section=header&text=Level%201%20%C2%B7%20Beginner&fontSize=52&fontColor=ffffff&fontAlignY=38&animation=fadeIn&desc=HTML%20%C2%B7%20Git%20%C2%B7%20CSS%20%C2%B7%20Responsive%20%C2%B7%20Tailwind&descSize=18&descAlignY=60" width="100%" alt="Level 1 Beginner" />

<img src="https://skillicons.dev/icons?i=html,css,git,github,tailwind,vscode" alt="HTML CSS Git GitHub Tailwind VS Code" />

<br /><br />

<img src="https://img.shields.io/badge/Weeks-1_→_8-EA580C?style=for-the-badge" alt="Weeks 1-8" />
<img src="https://img.shields.io/badge/Video-~23_h-F59E0B?style=for-the-badge" alt="About 23 hours of video" />
<img src="https://img.shields.io/badge/Main_Source-Elzero_Web_School-111827?style=for-the-badge" alt="Elzero Web School" />

<br /><br />

[Roadmap](README.md) · **Beginner** · [Intermediate](02-intermediate.md) · [React](03-react.md) · [Vue](03-vue.md) · [Tracker](TRACKER.md)

</div>

---

You'll build the **look**: pages that mean something (HTML), look good (CSS), work on any screen (Responsive), and get written ten times faster (Tailwind). From week 2 on, everything you build goes **live on the internet**.

| Week | Topic | You ship |
| :--: | :-- | :-- |
| [1](#week-1) | HTML basics | An "About Me" page |
| [2](#week-2) | Semantic HTML, forms, a11y + Git & GitHub | An event sign-up form, live |
| [3](#week-3) | CSS basics | A profile card |
| [4](#week-4) | Box model, position, Flexbox | Navbar + pricing cards |
| [5](#week-5) | Grid, transforms, animations | A dashboard layout |
| [6](#week-6) | Responsive design & modern CSS | A Frontend Mentor challenge |
| [7](#week-7) | Tailwind CSS | Pricing page in Tailwind + dark mode |
| [8](#week-8) | **Project 1** | A complete landing page |

---

<a id="week-1"></a>

## Week 1 · HTML Basics

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=6QAELgirvjs&list=PLDoPjvoNmBAw_t_XWUFbBX-c9MafPk9ji&index=1"><img src="https://img.youtube.com/vi/6QAELgirvjs/mqdefault.jpg" width="320" alt="Elzero HTML #01" /></a>
<br /><b>Elzero · HTML #01 → #18</b>
<br />2 h

</td>
<td valign="top">

**Watch:** [Elzero · HTML #01 → #18](https://www.youtube.com/watch?v=6QAELgirvjs&list=PLDoPjvoNmBAw_t_XWUFbBX-c9MafPk9ji&index=1) · **2 h**

**Goal:** write a full HTML page from scratch and know what every tag does.

**Topics:** page structure · headings & paragraphs · attributes · links & paths · images · lists · tables · `div` & `span` · entities

**Practice:** Elzero assignments [01-05](https://elzero.org/html-assignments-lesson-from-1-to-5/) · [06-10](https://elzero.org/html-assignments-lesson-from-6-to-10/) · [11-14](https://elzero.org/html-assignments-lesson-from-11-to-14/) · [15-18](https://elzero.org/html-assignments-lesson-from-15-to-18/)

**Read:** [Learn HTML · web.dev](https://web.dev/learn/html) · [Elements reference · MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

</td>
</tr>
</table>

#### Task · About Me page

Build `index.html` about yourself. **HTML only, no CSS.**

- Your name in an `h1` and a short bio
- A photo with a meaningful `alt`
- A list of hobbies and a numbered list of this year's goals
- A table of your weekly study schedule
- Links to your GitHub and LinkedIn that open in a new tab
- A second page, `hobbies.html`, linked both ways

> [!TIP]
> **Bonus:** use `colspan` and `rowspan` to rebuild your college timetable.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know the difference between an element, a tag, and an attribute
- [ ] I know why `alt` matters, and not just for SEO
- [ ] I know `./img.png` vs `/img.png` vs `../img.png`
- [ ] I know block vs inline elements
- [ ] I solved the Elzero assignments for lessons 1-18

</details>

> [!WARNING]
> **Pitfalls:** `<br>` for spacing (that's CSS's job) · picking headings by size instead of meaning (one `h1` per page) · closing tags in the wrong order.

> [!NOTE]
> **Mentor tip:** don't memorize tags. Write a lot and they stick. Forgot one? Open MDN. Senior devs do it every day.

<div align="right"><a href="#top">Top ↑</a> · <a href="#week-2">Week 2 →</a></div>

---

<a id="week-2"></a>

## Week 2 · Semantic HTML, Forms & a11y + Git & GitHub

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=xlQwlfvrDuI&list=PLDoPjvoNmBAw_t_XWUFbBX-c9MafPk9ji&index=19"><img src="https://img.youtube.com/vi/xlQwlfvrDuI/mqdefault.jpg" width="320" alt="Elzero HTML #19" /></a>
<br /><b>Elzero · HTML #19 → #37</b>
<br />2 h

</td>
<td valign="top">

**Watch:** [Elzero · HTML #19 → #37](https://www.youtube.com/watch?v=xlQwlfvrDuI&list=PLDoPjvoNmBAw_t_XWUFbBX-c9MafPk9ji&index=19) · **2 h**

**Goal:** write meaningful HTML, build a full form, and put your work live on GitHub.

**Topics:** semantic elements · audio, video, iframe · every form input · `label` · validation attributes · intro to accessibility & ARIA · `git init / add / commit / push / pull / clone` · **GitHub Pages**

**Also watch:** [Elzero · Git #01 → #06](https://www.youtube.com/watch?v=ACOiGZoqC8w&list=PLDoPjvoNmBAw4eOj58MZPakHjaO3frVMF&index=1) + [#09](https://www.youtube.com/watch?v=usjh4jj7_nQ&list=PLDoPjvoNmBAw4eOj58MZPakHjaO3frVMF&index=9) · 59 min

**Practice:** Elzero [19-23](https://elzero.org/html-assignments-lesson-from-19-to-23/) · [24-27](https://elzero.org/html-assignments-lesson-from-24-to-27/) · [28-30](https://elzero.org/html-assignments-lesson-from-28-to-30/) · [31-34](https://elzero.org/html-assignments-lesson-from-31-to-34/) · [35-37](https://elzero.org/html-assignments-lesson-from-35-to-37/)

**Read:** [Web forms · MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/HTML_forms) · [Learn Forms · web.dev](https://web.dev/learn/forms) · [GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)

</td>
</tr>
</table>

#### Task · Event sign-up form

A sign-up page for a CIS workshop or hackathon:

- `header` + `nav`, `main` with an About section, an agenda table, and a map or video (`iframe`), then a `footer`
- A form with name, email, phone (`pattern` for an 11-digit Egyptian number), college (`select`), year (`radio`), interests (`checkbox`), and a "why" `textarea`
- Every input has a connected `label` (`for` + `id`)
- Repo `cis-event-form`, **3+ meaningful commits**, live on **GitHub Pages**

**Submit** the repo and live links on the dashboard.

> [!TIP]
> **Bonus:** unplug your mouse. Can you fill and submit the form with only `Tab`, `Space`, and `Enter`? If not, fix it.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know why `<nav>` beats `<div class="nav">`
- [ ] I know `GET` vs `POST`
- [ ] I know why every input needs a `label`
- [ ] I know `add` vs `commit` vs `push`
- [ ] I can create a repo and push a project without the video
- [ ] My page is live on GitHub Pages

</details>

> [!WARNING]
> **Pitfalls:** one commit called `final` · dragging files onto github.com instead of using the terminal · `placeholder` instead of `label`.

> [!NOTE]
> **Mentor tip:** your GitHub *is* your CV. Recruiters look at it before your resume. From today, push everything.

<div align="right"><a href="#week-1">← Week 1</a> · <a href="#top">Top ↑</a> · <a href="#week-3">Week 3 →</a></div>

---

<a id="week-3"></a>

## Week 3 · CSS Basics

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=X1ulCwyhCVM&list=PLDoPjvoNmBAzjsz06gkzlSrlev53MGIKe&index=1"><img src="https://img.youtube.com/vi/X1ulCwyhCVM/mqdefault.jpg" width="320" alt="Elzero CSS #01" /></a>
<br /><b>Elzero · CSS #01 → #29</b>
<br />3.5 h

</td>
<td valign="top">

**Watch:** [Elzero · CSS #01 → #29](https://www.youtube.com/watch?v=X1ulCwyhCVM&list=PLDoPjvoNmBAzjsz06gkzlSrlev53MGIKe&index=1) · **3.5 h**

**Goal:** control any element's colors, fonts, spacing, and background.

**Topics:** syntax & selectors · naming · backgrounds · padding, margin, border · `display` · sizing & overflow · text & typography · units (`px`, `em`, `rem`, `%`, `vw`) · inheritance · `calc()`

**Practice:** Elzero [01-04](https://elzero.org/css-assignments-lesson-from-1-to-4/) · [05-08](https://elzero.org/css-assignments-lesson-from-5-to-8/) · [09-12](https://elzero.org/css-assignments-lesson-from-9-to-12/) · [13-16](https://elzero.org/css-assignments-lesson-from-13-to-16/) · [17-21](https://elzero.org/css-assignments-lesson-from-17-to-21/) · [22-26](https://elzero.org/css-assignments-lesson-from-22-to-26/) · [27-29](https://elzero.org/css-assignments-lesson-from-27-to-29/)

**Read:** [Learn CSS · web.dev](https://web.dev/learn/css) · [Values & units · MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Values_and_units) · [CSS reset · Josh Comeau](https://www.joshwcomeau.com/css/custom-css-reset/)

</td>
</tr>
</table>

#### Task · Profile card

Turn your week 1 page into a centered **profile card**:

- Round photo, name, title ("Frontend Developer in Progress"), short bio, social buttons
- A Google Font
- `rem` for font sizes and spacing
- A separate CSS file, no inline `style=""`
- Live on GitHub Pages

> [!TIP]
> **Bonus:** on hover, lift the card slightly and deepen its shadow.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know `padding` vs `margin`
- [ ] I know `em` vs `rem` and when to use each
- [ ] I understand specificity: why an id beats a class
- [ ] I know which properties inherit
- [ ] I can center a block horizontally with `margin: auto`

</details>

> [!WARNING]
> **Pitfalls:** `!important` to force things (it's a specificity problem) · fixed `height` everywhere · class names like `red-text` or `box1`. Name by purpose: `card-title`.

> [!NOTE]
> **Mentor tip:** DevTools is your best friend in CSS. Tweak values live in Elements, then copy the result into your code.

<div align="right"><a href="#week-2">← Week 2</a> · <a href="#top">Top ↑</a> · <a href="#week-4">Week 4 →</a></div>

---

<a id="week-4"></a>

## Week 4 · Box Model, Position & Flexbox

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=-q5IyjKkKSc&list=PLDoPjvoNmBAzjsz06gkzlSrlev53MGIKe&index=30"><img src="https://img.youtube.com/vi/-q5IyjKkKSc/mqdefault.jpg" width="320" alt="Elzero CSS #30" /></a>
<br /><b>Elzero · CSS #30 → #53</b>
<br />3.5 h

</td>
<td valign="top">

**Watch:** [Elzero · CSS #30 → #53](https://www.youtube.com/watch?v=-q5IyjKkKSc&list=PLDoPjvoNmBAzjsz06gkzlSrlev53MGIKe&index=30) · **3.5 h**

**Goal:** understand how elements take up space, and lay out anything in one direction with Flexbox.

**Topics:** `position` & `z-index` · pseudo-classes & pseudo-elements · border-radius & shadows · **box model** & `box-sizing` · transitions · margin collapse · **CSS variables** · **Flexbox**

**Practice:** Elzero [30-33](https://elzero.org/css-assignments-lesson-from-30-to-33/) · [34-37](https://elzero.org/css-assignments-lesson-from-34-to-37) · [38-41](https://elzero.org/css-assignments-lesson-from-38-to-41/) · [42-45](https://elzero.org/css-assignments-lesson-from-42-to-45/) · [46-53](https://elzero.org/css-assignments-lesson-from-46-to-53/) · **[Flexbox Froggy](https://flexboxfroggy.com/)** (all 24 levels)

**Read:** [Interactive Flexbox guide · Josh Comeau](https://www.joshwcomeau.com/css/interactive-guide-to-flexbox/) · [Flexbox guide · CSS-Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

</td>
</tr>
</table>

#### Task · Navbar + pricing cards

- A `sticky` navbar: logo left, links center, "Sign Up" right
- 3 pricing cards (Basic, Pro, Team). The middle one stands out with a "Most Popular" label (`::before` or `position: absolute`)
- All colors and spacing as **CSS variables** in `:root`
- Buttons with `:hover` and `:focus-visible` transitions
- **Flexbox only.** No `float`, no `position` for layout.

> [!TIP]
> **Bonus:** change one variable (`--primary`) and the whole page re-themes.

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know `relative` vs `absolute`, and what `absolute` is positioned against
- [ ] I know `content-box` vs `border-box`
- [ ] I know `justify-content` vs `align-items`
- [ ] I know exactly what `flex: 1` means
- [ ] I can center anything with Flexbox in two lines
- [ ] I finished Flexbox Froggy

</details>

> [!WARNING]
> **Pitfalls:** `position: absolute` for everything · `display: flex` on every div · forgetting `box-sizing: border-box` in your reset.

> [!NOTE]
> **Mentor tip:** play Flexbox Froggy twice: now, and again in a week without hints.

<div align="right"><a href="#week-3">← Week 3</a> · <a href="#top">Top ↑</a> · <a href="#week-5">Week 5 →</a></div>

---

<a id="week-5"></a>

## Week 5 · Grid, Transforms & Animations

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=2v9ZhqX6YOk&list=PLDoPjvoNmBAzjsz06gkzlSrlev53MGIKe&index=54"><img src="https://img.youtube.com/vi/2v9ZhqX6YOk/mqdefault.jpg" width="320" alt="Elzero CSS #54" /></a>
<br /><b>Elzero · CSS #54 → #82</b>
<br />4 h

</td>
<td valign="top">

**Watch:** [Elzero · CSS #54 → #82](https://www.youtube.com/watch?v=2v9ZhqX6YOk&list=PLDoPjvoNmBAzjsz06gkzlSrlev53MGIKe&index=54) · **4 h**

**Goal:** build two-dimensional layouts with Grid and bring pages to life with motion.

**Topics:** filters & gradients · **Grid** (`template-columns`, `template-areas`, `gap`, `minmax`, `auto-fill` / `auto-fit`) · 2D & 3D transforms · `@keyframes` animations · selectors in depth

**Practice:** Elzero [54-56](https://elzero.org/css-assignments-lesson-from-54-to-56/) · [57-64](https://elzero.org/css-assignments-lesson-from-57-to-64/) · [65-67](https://elzero.org/css-assignments-lesson-from-65-to-67/) · [68-73](https://elzero.org/css-assignments-lesson-from-68-to-73/) · [74-77](https://elzero.org/css-assignments-lesson-from-74-to-77/) · [78-82](https://elzero.org/css-assignments-lesson-from-78-to-82/) · **[Grid Garden](https://cssgridgarden.com/)** (all 28 levels)

**Read:** [Interactive Grid guide · Josh Comeau](https://www.joshwcomeau.com/css/interactive-guide-to-grid/) · [Grid guide · CSS-Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/)

</td>
</tr>
</table>

#### Task · Dashboard layout

Layout only, no functionality needed:

- Sidebar, header, and main area with `grid-template-areas`
- Main area: 4 stat cards, one wide "chart" card spanning 2 columns, and a "Recent activity" card
- Stat cards auto-flow with `repeat(auto-fit, minmax(200px, 1fr))`
- A pure-CSS loading spinner (`@keyframes`)
- Cards lift on hover with `transform`

> [!TIP]
> **Bonus:** a **flip card** that turns over on hover (3D transforms + `backface-visibility`).

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know when to use Flexbox and when to use Grid
- [ ] I know what `fr` means
- [ ] I know `auto-fill` vs `auto-fit`
- [ ] I know `transition` vs `animation`
- [ ] I know why animating `transform` and `opacity` is cheaper than `top` and `width`
- [ ] I finished Grid Garden

</details>

> [!WARNING]
> **Pitfalls:** using only Grid or only Flex. Rule of thumb: **Grid for page layout, Flex for components.** Too much animation annoys people, and some get physically uncomfortable.

> [!NOTE]
> **Mentor tip:** see a site you like? Open DevTools and see how its layout is built. You'll learn more than from any course.

<div align="right"><a href="#week-4">← Week 4</a> · <a href="#top">Top ↑</a> · <a href="#week-6">Week 6 →</a></div>

---

<a id="week-6"></a>

## Week 6 · Responsive Design & Modern CSS

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=F9FAcVwSV4c&list=PLDoPjvoNmBAzjsz06gkzlSrlev53MGIKe&index=83"><img src="https://img.youtube.com/vi/F9FAcVwSV4c/mqdefault.jpg" width="320" alt="Elzero CSS #83" /></a>
<br /><b>Elzero · CSS #83 → #88</b>
<br />1 h

</td>
<td valign="top">

**Watch:** [Elzero · CSS #83 → #88](https://www.youtube.com/watch?v=F9FAcVwSV4c&list=PLDoPjvoNmBAzjsz06gkzlSrlev53MGIKe&index=83) · **1 h**

**Goal:** every page you build looks right on phone, tablet, and laptop.

**Topics:** media queries & breakpoints · **mobile first** · viewport meta · responsive images (`max-width`, `object-fit`) · fluid sizes with `clamp()` · container queries · `:has()` · native CSS nesting

**Build along:** [Elzero · HTML & CSS Template 1](https://www.youtube.com/playlist?list=PLDoPjvoNmBAzHSjcR-HnW9tnxyuye8KbF) · 2 h. Your first full site built from scratch. Watch *how* he thinks, not just what he types.

**Practice:** Elzero [83-85](https://elzero.org/css-assignments-lesson-from-83-to-85/) · [86-88](https://elzero.org/css-assignments-lesson-from-86-to-88/)

**Read:** **[Learn Responsive Design · web.dev](https://web.dev/learn/design)** (the key read this week) · [Responsive design · MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Responsive_Design) · [Container queries · MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_containment/Container_queries)

</td>
</tr>
</table>

#### Task · Frontend Mentor challenge

1. Pick a free **Newbie** or **Junior** challenge with mobile and desktop designs from [Frontend Mentor](https://www.frontendmentor.io/challenges)
2. Build it **mobile first**
3. Make your week 4 pricing page and week 5 dashboard responsive too

**Submit** 3 live links.

> [!TIP]
> **Bonus:** a card that switches between stacked and side-by-side based on its **container** width, not the screen (container queries).

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I know why mobile first beats desktop first
- [ ] I know what breaks without the viewport meta tag
- [ ] I can make a font scale fluidly with `clamp()`
- [ ] I know media queries vs container queries
- [ ] I test with DevTools' device toolbar *and* a real phone

</details>

> [!WARNING]
> **Pitfalls:** a breakpoint for every phone model (add breakpoints where *your design* breaks) · horizontal scroll on mobile (usually a fixed `px` width or an image without `max-width: 100%`).

> [!NOTE]
> **Mentor tip:** most visitors to Egyptian websites are on phones. Mobile isn't the extra version; it's the main one.

<div align="right"><a href="#week-5">← Week 5</a> · <a href="#top">Top ↑</a> · <a href="#week-7">Week 7 →</a></div>

---

<a id="week-7"></a>

## Week 7 · Tailwind CSS

<table>
<tr>
<td width="340" valign="top">

<a href="https://www.youtube.com/watch?v=QJEd-99TA_A&list=PLdnrjoDUmGZ8Q9Dq9ebR9v1xEgqJ6tcfx&index=1"><img src="https://img.youtube.com/vi/QJEd-99TA_A/mqdefault.jpg" width="320" alt="Tailwind CSS 4 course" /></a>
<br /><b>Triangles · Tailwind CSS 4</b>
<br />3.5 h

</td>
<td valign="top">

**Watch:** [Triangles · Tailwind CSS 4](https://www.youtube.com/watch?v=QJEd-99TA_A&list=PLdnrjoDUmGZ8Q9Dq9ebR9v1xEgqJ6tcfx&index=1) · **3.5 h**

**Goal:** write CSS much faster with utility classes, and see why most React and Vue projects use Tailwind.

**Topics:** utility-first · installing Tailwind v4 with Vite · spacing, colors, typography · Flex & Grid utilities · `sm:` `md:` `lg:` · `hover:` `focus:` `dark:` · `@theme` · why `@apply` is a trap

**Read:** [Install with Vite](https://tailwindcss.com/docs/installation/using-vite) · **[Styling with utility classes](https://tailwindcss.com/docs/styling-with-utility-classes)** (read it all)

</td>
</tr>
</table>

> [!IMPORTANT]
> Tailwind **doesn't replace** knowing CSS. Every class is a CSS line you already know. If `flex justify-between items-center` isn't obvious to you, go back to week 4.
>
> You need **Node.js LTS** to run Vite. Just follow the install steps for now; npm and Vite get a full week in week 16.

#### Task · Pricing page in Tailwind + dark mode

- Rebuild your week 4 navbar + pricing cards **from scratch** in Tailwind
- Fully responsive
- A dark mode toggle (`dark:` + one line of JS: `document.documentElement.classList.toggle('dark')`)
- Custom colors in `@theme`
- Deploy on [Vercel](https://vercel.com) or [Netlify](https://www.netlify.com). GitHub Pages needs extra setup with Vite.

> [!TIP]
> **Bonus:** compare the final CSS file size of the Tailwind version and your plain CSS version. Which is smaller, and why?

<details>
<summary><b>Exit checklist</b></summary>

<br />

- [ ] I can translate any Tailwind class into plain CSS in my head
- [ ] I can set up Tailwind in a new Vite project without a video
- [ ] I know `md:flex` means "from md and up", not "only at md"
- [ ] I can add custom colors and fonts in `@theme`

</details>

> [!WARNING]
> **Pitfalls:** dynamic class names like `` `bg-${color}-500` `` (Tailwind can't see them) · `@apply` everywhere, which is just plain CSS the hard way.

> [!NOTE]
> **Mentor tip:** install the **Tailwind CSS IntelliSense** extension. It halves the time you spend hunting for class names.

<div align="right"><a href="#week-6">← Week 6</a> · <a href="#top">Top ↑</a> · <a href="#week-8">Week 8 →</a></div>

---

<a id="week-8"></a>

## Week 8 · Project 1: Landing Page

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:EA580C,100:F59E0B&height=90&text=Milestone%20Project%201&fontSize=34&fontColor=ffffff&animation=twinkling" width="100%" alt="Milestone Project 1" />

</div>

**Goal:** build a real landing page from a design, alone, with no video to follow. **Just you and the design.**

Pick one:
- A **Junior** or **Intermediate** landing page on [Frontend Mentor](https://www.frontendmentor.io/challenges)
- A landing page from [Figma Community](https://www.figma.com/community) with mobile and desktop frames

| Requirement | Details |
| :-- | :-- |
| **Sections** | 5+: navbar, hero, features, testimonials or pricing, footer |
| **Responsive** | Mobile first; works at 375 px, 768 px, and 1440 px |
| **Semantic HTML** | Right tags, one `h1` |
| **Accessibility** | `alt` everywhere, keyboard-friendly, readable contrast |
| **Styling** | Plain CSS or Tailwind, your call |
| **Git** | 10+ meaningful commits, none called `final` |
| **Deploy** | Live on GitHub Pages, Vercel, or Netlify |
| **README** | Screenshot, live link, tools used, hardest part |
| **Lighthouse** | **90+** in Accessibility and Best Practices |

**Submit** the repo, live link, and a Lighthouse screenshot.

> [!TIP]
> **Bonus:** dark mode · CSS-only scroll animations (`animation-timeline: view()`) · post your solution on Frontend Mentor for community feedback.

<details>
<summary><b>Level 1 exit checklist</b></summary>

<br />

- [ ] I can build any static page from a design on my own
- [ ] I think mobile first without trying
- [ ] I know Flex vs Grid at a glance
- [ ] My GitHub has 8+ live repos
- [ ] I can pull colors, fonts, and spacing out of a design
- [ ] When CSS breaks, I open DevTools and find out why

</details>

> [!WARNING]
> **Pitfalls:** copying from an Elzero template (peek if stuck, but make it *yours*) · chasing pixel-perfect until you quit (90% and finished beats 99% and not) · coding before planning. Spend 20 minutes splitting the design into sections first.

> [!NOTE]
> **Mentor tip:** this is the first thing in your portfolio. Build it like someone is paying you. Then have a friend open it on their phone and tell you the truth.

<div align="right"><a href="#week-7">← Week 7</a> · <a href="#top">Top ↑</a></div>

---

<div align="center">

### Level 1 done.

You can build any **static** page. But buttons don't do anything yet, forms don't check anything, and no data comes from anywhere. That's next.

<a href="02-intermediate.md"><img src="https://img.shields.io/badge/Next_→_Level_2:_Intermediate-CA8A04?style=for-the-badge" alt="Next: Level 2 Intermediate" /></a>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:F59E0B,100:EA580C&height=110&section=footer" width="100%" alt="" />

</div>
