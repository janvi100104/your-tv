# Contributing Guide

Thank you for considering contributing to Movie App!

## Development Setup
1. Fork & clone the repo
2. Install dependencies: `npm install`
3. Create `.env` with `VITE_TMDB_API_KEY=your_key`
4. Run the dev server: `npm run dev`

## Workflow
- Create a branch from `main`
- Keep PRs small and focused
- Reference issues: `Closes #12`

## Commit Convention
Use Conventional Commits:
`<type>(scope?): message`

Types: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`.

## PR Checklist
- Descriptive title
- Linked issue
- No console errors
- Screenshots/GIF for UI changes
- Updated docs if needed

## Testing Checklist (Manual)
- Search with valid/invalid input
- Loading state visible
- Error message on network failure
- Empty state (no results)
- Mobile layout check

## Code Style
- Functional components + hooks
- Avoid duplication
- Keep components small

## Security
Remove secrets before committing. Do not expose API keys.

## Questions?
Open an issue with label `question`.

Happy hacking!
