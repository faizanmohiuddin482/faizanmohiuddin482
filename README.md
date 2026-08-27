<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:6366F1,100:22D3EE&height=220&section=header&text=Mohammed%20Faizan%20Mohiuddin&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=Senior%20Full%20Stack%20Engineer%20%C2%B7%20React%2FNext.js%20%C2%B7%20AI%2FLLM%20Systems&descAlignY=58&descSize=18&animation=fadeIn" width="100%"/>

<a href="https://linkedin.com/in/mohd-faizan"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:faizanmohiuddin.dev@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<img src="https://img.shields.io/badge/Hyderabad%2C%20India-333333?style=for-the-badge&logo=googlemaps&logoColor=white"/>

</div>

```bash
$ whoami
faizan — senior full-stack engineer, building production AI infra & frontend platforms

$ cat philosophy.txt
Measure everything. Never guess when you can profile.
Architecture is a decision you make once and pay for forever — so make it deliberately.

$ ls ./currently/
architecting qureos-frontend/    shipping vargo.in/    open to Senior Frontend/Full-Stack roles/
```

<br/>

## 🏗️ Systems I've Actually Built

Not "I know React" — here's the real shape of two systems I designed and shipped in production.

<table>
<tr><td>

**Production LLM Evaluation Pipeline** (Qureos) — sustains 20+ concurrent AI evaluation jobs, zero downtime.

```mermaid
flowchart LR
    Req["Eval Request"] --> Q{{"Job Queue"}}
    Q --> Pool["API Key Pool"]
    Pool --> Call["LangChain → OpenAI GPT-4/5"]
    Call -->|error| Retry["Retry w/ Backoff"]
    Retry --> Pool
    Call -->|success| Cache[("Multi-Layer Cache")]
    Cache --> Out["Fit Score · Gap Analysis · Summary"]
```

</td></tr>
<tr><td>

**Greenfield Frontend Platform** (`qureos-frontend`) — dual-axis architecture, CI-enforced boundaries so it can't decay back into the "mix of components" it replaced.

```mermaid
flowchart TB
    subgraph FSD["apps/web — Feature-Sliced Design"]
        shared --> entities --> features --> widgets --> app
    end
    subgraph AD["packages/ui — Atomic Design"]
        shadcn --> wrapper --> atom --> molecule
    end
    spec[["api-v3 OpenAPI Spec"]] --> client["@qureos/api-client (generated)"]
    client --> zod["Zod boundary validation"] --> features
    molecule --> widgets
    ci{{"CI: ESLint boundaries + dependency-cruiser"}} -. enforces .-> shared
    ci -. enforces .-> shadcn
```

</td></tr>
</table>

<br/>

## 📈 Case Studies, Not Claims

<table>
<tr><td width="33%" valign="top">

**46% smaller, 25% faster**
<br/><br/>
*Problem:* app was shipping bloated bundles, slow first paint.
<br/>
*Approach:* led a system-wide audit — code-splitting, dependency pruning, targeted refactors.
<br/>
*Result:* 46% smaller bundle, 25% faster overall performance, org-wide.

</td><td width="33%" valign="top">

**20+ concurrent jobs, 0 downtime**
<br/><br/>
*Problem:* AI evaluation jobs bottlenecked on rate limits and flaky calls.
<br/>
*Approach:* architected API key pooling, retry logic, multi-layer caching, queue-based processing.
<br/>
*Result:* sustained 20+ concurrent jobs with zero downtime.

</td><td width="33%" valign="top">

**Architecture that can't decay**
<br/><br/>
*Problem:* legacy frontend was an unstructured "mix of components."
<br/>
*Approach:* authored ADRs for a two-axis structure (FSD + Atomic Design), enforced via CI dependency rules.
<br/>
*Result:* boundary violations fail the build — decay is structurally prevented, not just discouraged.

</td></tr>
</table>

<br/>

## 🧰 Skill Matrix

**Daily driver, production:** `React` `Next.js` `TypeScript` `Node.js` `Tailwind CSS` `HTML5/CSS3`
<br/>
**Also shipped with:** `Python` `LangChain` `OpenAI API` `AWS` `GCP` `Firebase` `PostgreSQL` `MongoDB` `Electron`

<div align="center">

<img src="https://skillicons.dev/icons?i=react,nextjs,ts,js,html,css,tailwind,nodejs,electron&theme=dark" /><br/>
<img src="https://skillicons.dev/icons?i=aws,gcp,azure,vercel,firebase,supabase,mongodb,postgres&theme=dark" /><br/>
<img src="https://skillicons.dev/icons?i=openai,git,github,vscode,figma,docker&theme=dark" />

</div>

<br/>

## 🚀 Shipped Solo, End-to-End

| Product | What it is | Live |
|---|---|---|
| **Vargo Logistics** | Multi-tenant logistics SaaS — Shopify integration, prepaid wallet | [vargo.in](https://vargo.in) |
| **FetchMate** | Privacy-first offline API client — Electron + browser ext + VS Code ext | [fetchmate.vercel.app](https://fetchmate.vercel.app) |
| **bullpen** ⭐ open source | Skills that make AI coding agents behave like senior engineers | [demo](https://faizanmohiuddin482.github.io/bullpen/) · [source](https://github.com/faizanmohiuddin482/bullpen) |
| **Memoria** | AI memory assistant — NL storage, semantic search via pgvector | [altmemoria.netlify.app](https://altmemoria.netlify.app) |

<br/>

## 📊 GitHub Activity

<div align="center">
<img height="165" src="https://github-readme-stats.vercel.app/api?username=faizanmohiuddin482&show_icons=true&count_private=true&theme=tokyonight&hide_border=true&title_color=22D3EE&icon_color=6366F1"/>
<img height="165" src="https://github-readme-streak-stats.herokuapp.com/?user=faizanmohiuddin482&theme=tokyonight&hide_border=true&ring=22D3EE&fire=6366F1"/>
</div>

<div align="center">
<img src="https://raw.githubusercontent.com/faizanmohiuddin482/faizanmohiuddin482/output/github-contribution-grid-snake.svg" width="95%"/>
</div>

<br/>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:22D3EE,100:6366F1&height=100&section=footer"/>
</div>
