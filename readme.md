# XAI-Ed @ LAK27

Website for XAI-Ed 2027: Closing the Interpretation-Action Loop — Actionable Explainable AI to Enhance Learning and Teaching, a full-day workshop at the 17th International Conference on Learning Analytics & Knowledge (LAK27), Recife, Brazil. Served at <https://www.xai-ed.net/LAK27/>.

## Site Structure

- **Homepage** — Banner with event details, invited talk and panel frames, motivation, goals, expected outcomes
- **Call for Papers** — Topics, review process, important dates
- **Keynote** — Invited talk
- **Panel** — Cross-stakeholder panel
- **Schedule** — Programme timetable
- **Proceedings** — Accepted papers
- **Organisers** — Organising committee profiles

## Getting Started

### Prerequisites

- [Hugo Extended v0.151+](https://gohugo.io/installation/)
- [Node v22+](https://nodejs.org/en/download/)
- [Go v1.24+](https://go.dev/doc/install)

### Install Dependencies

```bash
npm install
```

### Development

```bash
npm run dev
```

### Build

```bash
npm run build
```

## Customisation

| What | Where |
|---|---|
| Site title & base URL | `hugo.toml` |
| Logo, nav button, metadata | `config/_default/params.toml` |
| Navigation menus | `config/_default/menus.en.toml` |
| Colors & fonts | `data/theme.json` |
| Social links | `data/social.json` |
| Homepage content | `content/english/_index.md` |
| Schedule | `content/english/schedule.md` |
| Organisers | `content/english/organisers/` |

## Credits

Built with [Hugoplate](https://github.com/zeon-studio/hugoplate) — a Hugo + Tailwind CSS starter template by [Zeon Studio](https://zeon.studio/), released under the [MIT License](https://github.com/zeon-studio/hugoplate/blob/main/LICENSE).
