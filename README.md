<div align="center">

# IN SIHWAN

**SOFTWARE DEVELOPER**

**Hanyang University**  
Department of Information Systems

<br>

[![Gmail](https://img.shields.io/badge/ian24665003@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:ian24665003@gmail.com)
[![Naver Mail](https://img.shields.io/badge/ian5003@naver.com-03C75A?style=flat-square&logo=naver&logoColor=white)](mailto:ian5003@naver.com)
[![GitHub](https://img.shields.io/badge/vaxxerz-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/vaxxerz)

</div>

<br>

## 01 / ABOUT

I'm an Information Systems student at Hanyang University,
interested in building practical and scalable software.

My primary focus is backend engineering, with experience
in full-stack development, database architecture,
and turning ideas into working products — from mobile
apps to production websites that real businesses run on.

<br>

## 02 / SELECTED WORK

> Click **Details** under each project to expand the engineering notes.

<br>

### [HOWEON Corporate Website ↗](https://howeon-site.pages.dev/#/)

**Industrial Web · Real-time 3D Product Showcase · Client Project**

<p align="center">
  <a href="https://howeon-site.pages.dev/#/"><img src="assets/howeon/desktop-home.png" alt="HOWEON website — home with real-time 3D bar screen model" width="48%"></a>
  &nbsp;
  <a href="https://howeon-site.pages.dev/#/products/double-chain-bar-screen"><img src="assets/howeon/desktop-product-detail.png" alt="Product detail — interactive 3D double chain rotary bar screen" width="48%"></a>
</p>

A corporate website for a water-treatment equipment and plant engineering company.
Interactive Three.js models show how each machine works, while 34 products,
49 projects and 16 certifications are managed as structured content.

[![Live](https://img.shields.io/badge/Live-howeon--site.pages.dev-00C2FF?style=flat-square)](https://howeon-site.pages.dev/#/)
![Role](https://img.shields.io/badge/Role-Solo_Development-333?style=flat-square)
![Source](https://img.shields.io/badge/Source-Private_(client_work)-555?style=flat-square)

<details>
<summary><b>Details — Key Engineering & Technology</b></summary>

<br>

**Key Engineering**
- Migrated a monolithic vanilla JS page to a modular Vite build
  without changing the existing visuals (verified by 22-shot pixel diff)
- Real-time 3D product viewers with lazy-loaded model chunks,
  adaptive quality and WebGL failure fallbacks
- JSON content model with schema validation and reference checks
  across products, projects, certificates and patents
- Local admin tool for staff edits — scrypt auth, CSRF protection,
  upload validation, change history and restore
- Automated quality pipeline: unit tests, Playwright E2E on
  Chromium / WebKit / Firefox at 4 viewport widths, build output audit
- Mobile-first navigation and filtering, deployed on Cloudflare Pages

**Technology**
`JavaScript` · `Three.js` · `GSAP` · `Vite` · `Node.js` · `Playwright` · `GitHub Actions` · `Cloudflare Pages`

</details>

<br>

---

### [coordit ↗](https://github.com/ganadidududu/coordit)

**Fashion Technology · Measurement-based Fit Analysis · Team Project**

<p align="center">
  <img src="assets/coordit/wardrobe.png" alt="Closet with reference garment measurements" width="30%">
  &nbsp;
  <img src="assets/coordit/recommendation.png" alt="Fit Lab — recommended size, fit score and per-part differences" width="30%">
  &nbsp;
  <img src="assets/coordit/score-breakdown.png" alt="Score breakdown by size, silhouette and body part" width="30%">
</p>

An iOS & Android app that recommends the right size by comparing a product's
size chart with the measurements of clothes you already fit well —
instead of guessing what "M" means at each brand.

[![Repo](https://img.shields.io/badge/Repo-ganadidududu%2Fcoordit-181717?style=flat-square&logo=github)](https://github.com/ganadidududu/coordit)
![Role](https://img.shields.io/badge/Role-Backend_Development-333?style=flat-square)
[![iOS](https://img.shields.io/badge/iOS-App_Store-0D96F6?style=flat-square&logo=apple&logoColor=white)](https://apps.apple.com/kr/app/coordit/id6804425048)
![Android](https://img.shields.io/badge/Android-555?style=flat-square&logo=android&logoColor=white)

<details>
<summary><b>Details — Key Engineering & Technology</b></summary>

<br>

**Key Engineering**
- Deterministic Fit Score Engine — weighted, tolerance-normalized
  Huber loss across 11 garment categories
- Multi-garment reference profile using weighted median and
  Huber-corrected mean to reduce outlier impact
- REST API with Supabase token verification, per-user data scoping
  and owner-based RLS policies
- Atomic writes for closet, analysis and credit usage via
  SQL RPC with idempotency keys
- LLM-generated fit reports grounded in engine results,
  with validated fallback explanations
- Size-chart import from product URLs (Playwright · Cheerio)

**Technology**
`TypeScript` · `Node.js` · `Express` · `Zod` · `PostgreSQL` · `Supabase` · `Docker`

</details>

<br>

---

### [HY-WAY ↗](https://hy-way.vercel.app)

**Campus Navigation · Graph-based Pathfinding · Independent Project**

<p align="center">
  <img src="assets/hy-way/map-route.png" alt="Map view — normal route vs portal route from IT/BT to HIT" width="30%">
  &nbsp;
  <img src="assets/hy-way/route.png" alt="Route comparison — 11m 20s normal vs 7m 46s with 2 portals" width="30%">
  &nbsp;
  <img src="assets/hy-way/portal.png" alt="List of campus portals — shortcuts through buildings" width="30%">
</p>

A navigation service for Hanyang University's Seoul campus that finds
the routes students actually take — through buildings, stairs and elevators
("portals") that regular map apps don't know about.

[![Live](https://img.shields.io/badge/Live-hy--way.vercel.app-0064FF?style=flat-square)](https://hy-way.vercel.app)
[![Repo](https://img.shields.io/badge/Repo-vaxxerz%2FHY--WAY-181717?style=flat-square&logo=github)](https://github.com/vaxxerz/HY-WAY)
![Award](https://img.shields.io/badge/🏆_3rd_Place-FORIF_Hackathon-F5A623?style=flat-square)

<details>
<summary><b>Details — Key Engineering & Technology</b></summary>

<br>

**Key Engineering**
- Graph-based pathfinding over campus nodes and edges
- Side-by-side comparison of normal and portal-shortcut routes
- Accessibility-aware routing with slopes, stairs and elevators
- GPS start point snapped to the nearest graph node
- Building-based community and route reports on Supabase,
  storing distance only — never exact coordinates

**Technology**
`JavaScript` · `Vite` · `Kakao Maps API` · `Supabase` · `Vercel`

</details>

<br>

## 03 / TECHNICAL STACK

<table>
  <tr>
    <td><b>Languages</b></td>
    <td><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"> <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript"> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"> <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white" alt="SQL"> <img src="https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black" alt="C"> <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++"> <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white" alt="Java"></td>
  </tr>
  <tr>
    <td><b>Frontend</b></td>
    <td><img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"> <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"> <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite"> <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS"> <img src="https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white" alt="Three.js"> <img src="https://img.shields.io/badge/GSAP-88CE02?style=flat-square&logo=greensock&logoColor=black" alt="GSAP"></td>
  </tr>
  <tr>
    <td><b>Backend</b></td>
    <td><img src="https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js"> <img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white" alt="Express"> <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI"> <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT"></td>
  </tr>
  <tr>
    <td><b>Database</b></td>
    <td><img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"> <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white" alt="Supabase"> <img src="https://img.shields.io/badge/MariaDB-003545?style=flat-square&logo=mariadb&logoColor=white" alt="MariaDB"></td>
  </tr>
  <tr>
    <td><b>Infra &amp; Tools</b></td>
    <td><img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker"> <img src="https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white" alt="Vercel"> <img src="https://img.shields.io/badge/Cloudflare_Pages-F38020?style=flat-square&logo=cloudflarepages&logoColor=white" alt="Cloudflare Pages"> <img src="https://img.shields.io/badge/Cloud_Run-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="Cloud Run"> <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions"> <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" alt="Playwright"></td>
  </tr>
</table>

<br>

## 04 / CURRENT INTERESTS

Backend Architecture · Full-Stack Engineering  
AI-Powered Applications · Database Systems

<br>

---

<div align="center">

**IN SIHWAN**

Hanyang University · Information Systems

[ian24665003@gmail.com](mailto:ian24665003@gmail.com) · [ian5003@naver.com](mailto:ian5003@naver.com) · [GitHub](https://github.com/vaxxerz)

<sub>Designed with simplicity in mind.</sub>

</div>
