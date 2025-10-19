# LibreTube

> A privacy-first, lightweight YouTube frontend and media explorer — fast, minimal, and made for people who want control over how they watch and share video.

LibreTube (Libertube) is a modern client focused on speed, privacy, and simplicity. It strips away clutter, provides optional integrations, and keeps your data where it belongs — with you.

---

Status: WIP — fresh README to help contributors, users, and maintainers get started quickly.

Quick links
- Repository: https://github.com/Tarun-0213/Libertube
- License: MIT (see LICENSE)

---

Features
- Lightweight UI optimized for performance and accessibility
- Privacy-first by default (no tracking, opt-in integrations)
- Fast search and discovery with a minimal UX
- Support for playback via embedded players or external players
- Themable and extensible — easy to add plugins or UI tweaks
- Designed for both desktop and mobile

Why LibreTube?
- Clean, distraction-free watching experience
- No forced sign-ins, no tracking by default
- Easy to self-host or run locally
- Built to be extendable and community-driven

Screenshots / Demo
- Add screenshots or an animated GIF in /assets once available. Example: docs/demo.gif

Quickstart (local)
1. Prerequisites
   - Node.js 18+ (or the repo-specified node)
   - npm, yarn or pnpm
   - Optional: Docker & docker-compose for containerized runs

2. Clone
   git clone https://github.com/Tarun-0213/Libertube.git
   cd Libertube

3. Install
   npm install
   # or
   yarn
   # or
   pnpm install

4. Environment
   - Copy the example env file and edit as needed:
     cp .env.example .env
   - Typical variables:
     - PORT=3000
     - API_BACKEND_URL= (optional)
     - PLAYER=embedded|external

5. Run (development)
   npm run dev
   # or
   yarn dev
   Open http://localhost:3000

6. Build (production)
   npm run build
   npm start
   # or
   yarn build && yarn start

Docker (optional)
- Build
  docker build -t libretube:latest .
- Run
  docker run -p 3000:3000 --env-file .env libretube:latest

Configuration & Privacy
- LibreTube ships with privacy-first defaults. Integrations that may share data (analytics, third-party APIs) are disabled or opt-in.
- Review /docs/PRIVACY.md (or create it) to list all telemetry and external services.
- You can configure different playback backends (embedded, Invidious, PeerTube, external players) via configuration and environment variables.

Development notes
- Code style: follow the project's lint rules (eslint/prettier) — run npm run lint
- Tests: add unit and integration tests — run npm test
- Keep changes small and well-documented; use feature branches and open pull requests

Contributing
We welcome contributions of all sizes — bug fixes, docs, UX improvements, and feature proposals.
- Read CONTRIBUTING.md for the contribution workflow and guidelines.
- File issues for bugs and feature requests; use small, focused PRs.
- Be respectful and follow the CODE_OF_CONDUCT.md.

Roadmap (high level)
- Improve search relevance and caching
- Add optional offline playback / queue
- Plugin system for integrations (Invidious, PeerTube, etc.)
- Accessibility improvements and keyboard-first navigation
- Mobile-first layout optimizations

Maintainers & Contributors
- Repo owner: Tarun-0213
- Please add yourself to CONTRIBUTORS.md if you make contributions you'd like acknowledged.

Support & Contact
- Open an issue on GitHub for bugs, feature requests, or help.
- For quick questions, open a short discussion or use the PR comment threads.

License
- MIT — see LICENSE for full details.

Acknowledgements
- Inspiration and ideas from privacy-first media frontends and the OSS community.
- Thank you to contributors, testers, and users helping shape LibreTube.

Appendix: Helpful developer commands
- Start dev server: npm run dev
- Build: npm run build
- Start production server: npm start
- Lint: npm run lint
- Test: npm test

If anything in this README doesn't match the repository structure, tell me which files or scripts exist and I will update this README to match exactly.`  `  
