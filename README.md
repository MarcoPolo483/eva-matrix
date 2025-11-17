# 🚀 EVA Matrix - Public Landing Page

**Live Site**: https://marcopolo483.github.io/eva-matrix/ *(pending GitHub Pages setup)*

## What is EVA Matrix?

**EVA Matrix** is the public-facing landing page for **EVA 2.0** (Enterprise Virtual Assistant), an AI-powered platform built transparently by AI agents.

Unlike traditional software development that hides the process, **EVA Matrix shows everything**:
- ✅ Real-time sprint progress
- ✅ Quarterly roadmap (Q1-Q4 2026 + 2027 moonshots)
- ✅ Live demo links (coming Sprint 01 Week 2)
- ✅ Public Power BI dashboard embed (EVA Matrix metrics)

---

## 🌐 Enabling GitHub Pages

### Step 1: Enable GitHub Pages (One-Time Setup)

1. Go to repository **Settings** → **Pages**
2. Under **Source**, select:
   - **Branch**: `master`
   - **Folder**: `/docs`
3. Click **Save**
4. Wait ~2 minutes for deployment
5. Your site will be live at: **https://marcopolo483.github.io/eva-matrix/**

### Step 2: Verify Deployment

```powershell
# Check GitHub Pages status
gh browse --repo MarcoPolo483/eva-matrix --settings

# Or visit directly
start https://github.com/MarcoPolo483/eva-matrix/settings/pages
```

---

## 📁 Repository Structure

```
eva-matrix/
├── docs/
│   ├── index.html       ← Landing page (public)
│   ├── roadmap.html     ← Coming soon (Q1-Q4 2026 roadmap)
│   ├── demo.html        ← Coming soon (live demo iframe)
│   └── assets/          ← Coming soon (CSS, JS, images)
├── README.md            ← This file
└── .gitignore
```

---

## 🔒 Public vs. Private

| Content | Location | Access |
|---------|----------|--------|
| **Public Landing Page** | `eva-matrix` repo (GitHub Pages) | Anyone on the internet |
| **Live Demo Links** | Vercel/Azure Static Web Apps | Anyone (read-only preview) |
| **Public Power BI** | Embedded in `eva-matrix` landing page | Anyone (EVA Matrix dashboard only) |
| **Private MARCO HUB** | `eva-orchestrator` repo (Azure Static Web Apps) | Authorized users only (Entra ID) |
| **Private Power BI** | Embedded in MARCO HUB HTML | Authorized users only (7 dashboards) |
| **Architecture Docs** | `eva-orchestrator` repo (private) | Collaborators only |

---

## 🎨 Design Philosophy

**Inspired by**: Apple product launches, GitHub project pages, startup landing pages

**Key Elements**:
- Clean, modern design (Segoe UI, blue gradient)
- Sticky navigation (quick jump to sections)
- Real-time stats cards (days to go-live, sprint progress)
- Quarterly roadmap with milestones
- "Building an airplane while flying it" tagline
- Footer with GitHub org link and Canada AI Guidelines reference

---

## 📊 Live Progress Updates

**Manual Updates** (Sprint 01):
- Edit `docs/index.html` directly
- Update stats cards, milestone list, roadmap status
- Commit and push to GitHub (auto-deploys to Pages)

**Automated Updates** (Sprint 01 Week 2+):
- GitHub Actions pipeline (hourly cron job)
- Fetches sprint metrics from GitHub API
- Updates HTML via template + data injection
- Commits and pushes changes automatically

---

## 🚀 Next Steps

### Sprint 01 Week 1 (Nov 17-23, 2025)
- ✅ **DONE**: Create `eva-matrix` repo + landing page
- ✅ **DONE**: Enable GitHub Pages (manual setup required)
- 🚧 **TODO**: Update stats cards daily (manual until Week 2)

### Sprint 01 Week 2 (Nov 24-30, 2025)
- 🚧 **TODO**: Add Power BI embed (EVA Matrix dashboard)
- 🚧 **TODO**: Create GitHub Actions pipeline (hourly updates)
- 🚧 **TODO**: Add live demo iframe links (Vercel previews)

### Sprint 02+ (Dec 2025+)
- Add `/roadmap.html` page (interactive timeline)
- Add `/demo.html` page (embedded demos)
- Add `/assets/` folder (custom CSS, JS, images)
- Custom domain (optional): `eva-matrix.com`

---

## 📝 Updating the Landing Page

### Manual Update (Current Method)

```powershell
# Navigate to eva-matrix repo
cd 'c:\Users\marco\Documents\_AI Dev\Repos\eva-matrix'

# Edit index.html (update stats, milestones, roadmap)
# Save changes

# Commit and push
git add docs/index.html
git commit -m "📊 Update live progress - Sprint 01 Day X"
git push

# Wait ~2 minutes, then refresh https://marcopolo483.github.io/eva-matrix/
```

### Automated Update (Sprint 01 Week 2+)

GitHub Actions will update stats automatically every hour:
- Fetches sprint metrics from GitHub API
- Updates HTML stats cards
- Commits and pushes changes
- No manual intervention required

---

## 🔗 Links

- **Public Site**: https://marcopolo483.github.io/eva-matrix/ *(coming soon)*
- **GitHub Repo**: https://github.com/MarcoPolo483/eva-matrix
- **GitHub Org**: https://github.com/MarcoPolo483
- **Private Orchestrator**: https://github.com/MarcoPolo483/eva-orchestrator *(collaborators only)*
- **MARCO HUB**: `eva-orchestrator/docs/marco-hub.html` *(coming Sprint 01 Week 2: Azure Static Web Apps)*

---

## 📄 License

MIT License (or specify your preferred license)

---

**Last Updated**: November 17, 2025  
**Status**: ✅ Landing page created, GitHub Pages setup pending
