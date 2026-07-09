HELMSITE — complete ready-to-run Hugo site
==========================================
Already includes: PaperMod theme, helm design, config, sample content.
Verified building on Hugo v0.147.9.

RUN IT (3 commands):
  1. unzip helmsite.zip
  2. cd helmsite
  3. hugo server -D
  Open http://localhost:1313

REQUIREMENT:
  hugo version must be v0.146.0 or newer. Check: hugo version
  If older, install latest: https://gohugo.io/installation/

CHANGES YOU MUST MAKE (search "YOUR_" in these 2 files):
  hugo.yaml            -> your real GitHub + LinkedIn URLs (social icons)
  layouts/home.html    -> same 2 URLs for the wheel handles (marked TODO)

WHERE YOUR REAL CONTENT GOES:
  content/blog/       your posts (.md files) — samples included, delete them
  content/projects/   your projects — set "featured: true" to show on home
  content/docs/       your docs
  content/about.md    your about page

DEPLOY LATER:
  Set baseURL in hugo.yaml to your real domain before deploying.
