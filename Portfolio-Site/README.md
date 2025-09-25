# Portfolio-Site

Personal CV & portfolio website for **Theolen Pillay**.  
Clean, fast, and interview-ready: showcases projects, skills, experience, and a downloadable CV.

![Cover](../docs/screenshots/Portfolio-Site-cover.png)

---

## ✨ Highlights
- **Hero + Tagline** with quick CTAs (View CV, Contact)
- **Projects Gallery** linking to repos and case studies
- **Career Timeline** (internships, roles, education)
- **Skills Matrix** (languages, frameworks, cloud, tools)
- **Dark/Light Mode** toggle with logo theming
- **Downloadable CV (PDF)** button
- **Contact Section** (mailto or backend form)
- Mobile-first, accessible, and fast

---

## 🧱 Tech Stack
- **ASP.NET Core MVC (.NET 8)**, Razor Views  
- **Bootstrap 5** + custom CSS  
- Optional: **Tag Helpers**, **View Components**, **Partial Views**  
- (Alternative static build is possible if you decide to go pure HTML/CSS)

> If your site is static HTML/CSS: keep the sections below and ignore .NET commands.

---

## 🗂 Suggested Structure
/Portfolio-Site
/Controllers
/Models
/Views
/Shared
_Layout.cshtml
_Navbar.cshtml
_Footer.cshtml
Index.cshtml # Home (hero, highlights)
Projects.cshtml # Projects gallery
Timeline.cshtml # Career timeline
Contact.cshtml # Contact form / links
/wwwroot
/css/site.css
/img/
logo-light.png
logo-dark.png
headshot.jpg
/docs
cv/Theolen_Pillay_CV.pdf



---

## 🚀 Quick Start (ASP.NET Core)
### Prerequisites
- .NET 8 SDK installed

### Run (dev)
```bash
dotnet restore
dotnet run

App starts on https://localhost:****. Open in your browser.

Publish (local)
dotnet publish -c Release -o ./publish

🌐 Deployment Options
1) Azure App Service (recommended for MVC)

Create App Service → .NET 8 runtime

Deploy via publish folder or GitHub Actions

2) Static Hosting (if pure HTML/CSS)

GitHub Pages / Netlify / Vercel

Put built static files in /docs or root and enable Pages

🧩 Content Configuration

Projects: link to your monorepo subfolders

AgriEnergyConnect → /AgriEnergyConnect

MeetMeWhere → /MeetMeWhere

MemeStream (App/API) → /MemeStream-App, /MemeStream-API

OmnicoreMeetingMinutes → /OmnicoreMeetingMinutes

CV Button: link /docs/cv/Theolen_Pillay_CV.pdf

Contact:

Simple: mailto:your@email link

Advanced: Controller action + DB/email (optional)

🎨 Dark/Light Mode Notes

Use a theme toggle button (adds data-theme="dark" on <html>)

Swap logo based on theme:

logo-light.png for light theme

logo-dark.png for dark theme

Prefer CSS prefers-color-scheme as a default:

@media (prefers-color-scheme: dark) {
  .logo--light { display: none; }
  .logo--dark  { display: inline; }
}

♿ Accessibility & SEO

Semantic headings (H1 on home), alt text on images

Sufficient color contrast

Meta tags:

<meta name="description" content="Theolen Pillay — Software Developer. ASP.NET, Kotlin, Node.js.">
<meta property="og:title" content="Theolen Pillay — Portfolio">
<meta property="og:image" content="/img/og-cover.png">
<meta name="viewport" content="width=device-width, initial-scale=1">

🔧 Developer Notes

Use partial views for Navbar/Footer to keep pages tidy

Add a Projects card partial to reuse a clean card UI

Keep images optimized (≤ 200 KB where possible)

🧪 Checks (optional but pro)

Lint CSS (stylelint) and run dotnet build in CI

Add simple Playwright or Selenium smoke test (optional)

🧭 “Show me in 60 seconds” (Interview Demo Script)

Land on Home: tagline + quick CTAs

Toggle dark/light → show logo swap

Open Projects → click AgriEnergyConnect repo

Open Timeline → highlight internship/role

Click Download CV → opens PDF

Show Contact options (mailto or form)