# Design and Planning of Game — Economic Empire VI: Market City
**Student:** Tarek Barhoum  
**School:** Colegio Bolívar  
**Course:** AI Agents of Change  
**Subject:** AP Microeconomics  
**Level:** High School (Grades 11–12)  
**Curricular focus:** Scarcity and opportunity cost; supply and demand; marginal analysis; perfect competition; price ceilings.

## Super Prompt #1 — Project Declaration (Role + Context + Task + Conditions)
**Role:** Act as a senior educational game designer, AP Microeconomics instructor, and front-end web developer.
**Context:** I am an 11th-grade Colegio Bolívar student building an educational game for my AI Agents of Change course.
**Task:** Create an original browser-based, GTA-inspired top-down city exploration game called Economic Empire VI: Market City, teaching five AP Microeconomics concepts through interactive business missions.
**Conditions:** Use only HTML, CSS, and vanilla JavaScript, separated into index.html, style.css, and actions.js. Provide WASD/arrow movement and touch controls, five missions, a starting balance of $10,000, instant explanations, XP and cash rewards, a progress tracker, a game ending, and a visible external Google Forms evaluation link opening in a new tab. Make it responsive and compatible with GitHub Pages. Use original art and a fictional city; do not copy GTA assets.

## Game Declaration — AI Response
**Title:** Economic Empire VI: Market City.  
**Core mechanic:** Players explore a fictional coastal city in a top-down view. Each glowing business triggers a multiple-choice economic scenario.  
**Rules:** Start with $10,000. Approach a business and press E. Choose one of three options. A correct answer completes the mission, awards 1,000 XP and a cash bonus ($1,200–$3,500). A wrong answer deducts $500 and 200 XP, displays an explanation, and leaves the mission available to retry.  
**Win condition:** Complete all five missions.  
**Learning objectives:** Identify opportunity cost, predict demand shifts, compare marginal revenue and marginal cost, apply the perfectly competitive firm's profit-maximizing condition, and recognize shortages under binding price ceilings.  
**User experience:** Responsive neon city map, labeled buildings, instructions, accessible clickable answer choices, live financial HUD, touch controls, and a survey button.  
**Scoring:** Correct +1,000 XP; incorrect -200 XP (minimum zero); starting capital $10,000.  
**Educational feedback:** Every question gives a short concept explanation after an answer.

## Super Prompt #2 — Branch Development Plan (Role + Context + Task + Conditions)
**Role:** Act as a senior software engineer and Git workflow coach.
**Context:** I am implementing Economic Empire VI as an individual school project in one hour using GitHub Pages.
**Task:** Break the implementation into sequential Git feature branches, each independently testable, with clear commit messages and merges into main.
**Conditions:** Start each branch from main, commit only its feature, merge it back to main, push main before starting the next branch, and keep index.html/style.css/actions.js modular. Include Google Forms UX feedback in the final iteration.

## AI-Generated Iteration Plan
| Order | Git branch | Feature | Suggested commit |
|---|---|---|---|
| 1 | feature/game-interface | Main menu, map, HUD, styling | Build city interface and player HUD |
| 2 | feature/economic-engine | Player movement, money, score, mission triggers | Add player movement and economic engine |
| 3 | feature/game-levels | Five AP Microeconomics questions and decisions | Add five educational missions |
| 4 | feature/graphs-feedback | Immediate explanations, progress and game ending (optional graphs as future enhancement) | Add mission feedback and progress |
| 5 | feature/ux-evaluation | Survey link, mobile controls, polish | Integrate UX survey and mobile controls |

**Implementation note:** This starter package includes a complete playable final version. To show authentic incremental development in Git, create and commit each feature on its planned branch as you build or split the starter code; do not fabricate a development history. Interactive graphs are a future enhancement, not part of the current playable build.

## Google Form — Economic Empire VI: Player Experience Survey
Create the following six questions in Google Forms:
1. How clear were the game instructions? (Linear scale 1–5)
2. How visually appealing was the city and interface? (Linear scale 1–5)
3. How engaging were the missions? (Linear scale 1–5)
4. Did you learn something about AP Microeconomics? (Yes / Somewhat / No)
5. Which mission was your favorite? (Sunset Café / Ocean Mall / Neon Factory / Skyline Tower / City Hall)
6. What should be improved? (Paragraph)

Paste your real response-form link into `FORM_URL` in `actions.js`. Ask at least five real students to play and submit the form.

## How to Run Locally
1. Create/open the folder `ai-projects/economic-empire-vi` in VS Code.
2. Keep `index.html`, `style.css`, and `actions.js` in the same folder.
3. Open `index.html` using Live Server or a browser.
4. Walk with WASD or arrow keys; press E near a marker. Mobile users can tap the arrow and ENTER buttons.
5. Replace `FORM_URL` in `actions.js` with your actual Google Form responder URL.

## GitHub Commands — Initial Setup
```bash
git init -b main
git add index.html style.css actions.js PROJECT_DOCUMENTATION.md
git commit -m "Initialize Economic Empire VI project"
gh repo create economic-empire-vi --public --source=. --remote=origin --push
```
If the GitHub CLI is not authenticated, run `gh auth login` first. If the repo already exists, use its URL with `git remote add origin <repo-url>` and `git push -u origin main` instead.

## Feature Branch Workflow (repeat for each planned branch)
```bash
git switch main
git pull origin main
git switch -c feature/game-interface
# Make the specific feature changes, test with Live Server
git add .
git commit -m "Build city interface and player HUD"
git switch main
git merge feature/game-interface
git push origin main
```
Use each exact branch name and matching functionality from the plan. **Do not create empty commits or claim work happened on branches if it did not.**

## GitHub Pages Deployment
1. Open your GitHub repository.
2. Select Settings > Pages.
3. Choose Deploy from a branch > main > /(root) > Save.
4. Open the published URL and test movement, all five missions, ending, and survey button.

## Testing Checklist
- [ ] The game loads in a browser.
- [ ] WASD and arrow movement work.
- [ ] All five missions can be completed.
- [ ] Correct and incorrect answers show explanations.
- [ ] Money, XP, and progress update.
- [ ] Touch controls work on a phone.
- [ ] Survey opens the actual Google Form in a new tab.
- [ ] At least five students submit real survey responses.
- [ ] GitHub Pages loads the game without errors.

## Official Project Links (fill after publishing)
- **Public GitHub Repository:** [PASTE REAL URL]
- **GitHub Pages Application:** [PASTE REAL URL]
- **Google Form (grant teacher access to responses):** [PASTE REAL URL]

**Submission:** Submit only the final Google Doc containing this documentation and the three real URLs in Google Classroom. Confirm teacher access. Do not submit fake links or responses.
