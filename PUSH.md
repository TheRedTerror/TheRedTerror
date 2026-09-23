# Publish this profile README to GitHub

Your GitHub username is **TheRedTerror**. There is no profile README repo yet (`TheRedTerror/TheRedTerror` returns 404). This folder is ready to push.

## Current local state (verified)

| Check | Status |
| --- | --- |
| Branch | `main` |
| Working tree | Clean |
| Latest commit | `5021af6` — Align cyberpunk theme with profile picture palette |
| Remote `origin` | `git@github.com:TheRedTerror/TheRedTerror.git` *(already added)* |
| SSH auth | Works (`Hi TheRedTerror! You've successfully authenticated`) |
| GitHub repo | **Does not exist yet** (404) |

## 1. Create the profile repo on GitHub *(one-time, manual)*

GitHub requires the empty repo to exist before the first push. No API token or `gh` login is configured on this machine, so create it in the browser:

1. Open https://github.com/new
2. **Repository name:** `TheRedTerror` (must match your username exactly)
3. **Description:** `z3r0 — NetPhantom Security profile`
4. **Public**
5. Do **not** add a README, license, or `.gitignore` (this repo already has them)
6. Click **Create repository**

## 2. Push from this machine

Once the repo exists on GitHub, run:

```bash
cd /home/kali/Projects/TheRedTerror
git push -u origin main
```

SSH is already configured and the remote is set. No commit or remote setup needed.

If SSH fails, switch to HTTPS:

```bash
git remote set-url origin https://github.com/TheRedTerror/TheRedTerror.git
git push -u origin main
```

### Optional: use `gh` CLI for future updates

Install without sudo:

```bash
curl -sL "https://github.com/cli/cli/releases/download/v2.101.0/gh_2.101.0_linux_amd64.tar.gz" \
  | tar -xz -C /tmp/gh-install --strip-components=1
/tmp/gh-install/bin/gh auth login
```

To create and push in one step next time (after `gh auth login`):

```bash
gh repo create TheRedTerror/TheRedTerror --public --source=. --remote=origin --push
```

## 3. Verify

After push, confirm:

- Repo: https://github.com/TheRedTerror/TheRedTerror
- Profile README renders at: https://github.com/TheRedTerror

## 4. GitHub profile settings (manual)

At https://github.com/settings/profile:

| Field | Suggested value |
| --- | --- |
| **Name** | `z3r0` *(already set on your public profile)* |
| **Bio** | Red Team & Threat Intel Lead @ NetPhantom Security · adversary simulation · threat intel · low-noise, high-impact testing |
| **Company** | NetPhantom Security |
| **Website** | https://netphantomsecurity.com/ |
| **Location** | *(optional)* |
| **Pronouns** | *(optional)* |

## 5. Pin repositories

On https://github.com/TheRedTerror, click **Customize your pins** and consider:

1. `papa-prep-kit` — AI/agentic pentest prep (strongest original work)
2. `MysticalCTF` — Rust CTF platform
3. `pajaMAS` — MAS hijacking research
4. `it-depends` — SBOM / dependency tooling
5. `Portfolio` — if you refresh it for NetPhantom branding
6. *(optional)* fork or link your Z3r0 workbench if you own `yv1ing/Z3r0` or publish under this account

## 6. Optional polish

- **Profile picture:** NetPhantom / operator-themed avatar (void-dark palette, neon cyan/magenta accents)
- **Social preview:** Settings → General → Social preview → upload 1280×640 banner with NetPhantom + z3r0 branding
- **Banner image:** Replace the capsule-render header in `README.md` with a custom `assets/banner.png` hosted in this repo once you have artwork

## Brand reference

- Tagline: *You're not chasing shadows; We're chasing you.*
- Palette (cyberpunk): `#0a0a0f` / `#0d0221` void backgrounds · `#00fff5` cyan · `#ff00ff` magenta · `#a855f7` electric purple · `#39ff14` neon green
- Voice: operator, evidence-first, adversarial mindset — aligned with [NetPhantom team bio](https://netphantomsecurity.com/team/)
- Aesthetic: terminal/hacker, glitch-neon, SYSTEM ONLINE operator vibe
