# Contributing to Movie App

Thanks for your interest in improving the project! Follow these guidelines to keep the workflow smooth.

## Quick Start
1. Fork the repo
2. Clone your fork
3. Create a branch: `git checkout -b feat/short-description`
4. Install deps: `npm install`
5. Create `.env` with:
   ```env
   VITE_TMDB_API_KEY=your_key_here
   ```
6. Run dev server: `npm run dev`
7. Commit + push, open a Pull Request (PR)

## Branch Naming
- Features: `feat/<summary>`
- Fixes: `fix/<issue-number>-<summary>`
- Chore/infra: `chore/<summary>`

## Commit Messages (Conventional)
Format: `type(scope?): message`
Types: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`.
Examples:
- `feat(search): add debounced input`
- `fix(api): handle 500 errors gracefully`

## Coding Standards
- React + Vite (ES modules only)
- Keep components small & focused
- Prefer functional components + hooks
- Avoid unnecessary re-renders (memoize when justified)
- Use semantic HTML where possible
- Keep assets in `src/assets/`

## Environment & APIs
- TMDb API key required in `.env`
- Appwrite config lives in `src/appwrite.js` (mask secrets before committing)

## Adding a Feature
1. Open/confirm an issue (or create one) describing the change
2. Implement in a dedicated branch
3. Add/adjust README or inline docs if behavior changes
4. Manually test loading, error, empty, and mobile states
5. Ensure no console errors

## Pull Request Checklist
- Descriptive title
- Linked issue (e.g., `Closes #12`)
- Screenshots/GIFs for UI changes
- No unrelated file churn
- No hard‑coded secrets

## Reporting Issues
Include:
- Summary
- Steps to reproduce
- Expected vs actual
- Environment (OS, browser)
- Screenshots/logs if relevant

## Style / Tooling
- Run linters/formatters if configured
- Keep dependencies minimal

## Security
Never commit API keys or Appwrite credentials.

## License
By contributing, you agree your contributions are licensed under the repository’s MIT license.

## Need Help?
Open an issue with the label `question`.

Thank you for contributing!
