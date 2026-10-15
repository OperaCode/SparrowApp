# Contributing to Sparrow

This repository is the mobile app. The API lives in [OperaCode/Sparrow-backend](https://github.com/OperaCode/Sparrow-backend) and has its own setup.

## Getting started

Prerequisites:

- Node.js 22 and npm
- The Expo Go app on a device, or an Android/iOS simulator

```bash
npm install
cp .env.example .env
npm run dev
```

`lib/mockData.ts` is temporary demo data that powers the customer UI until the API is integrated. Don't build new production logic on top of it.

## Workflow

1. **Start from an issue.** Pick an open issue, and comment on it so others know you're working on it.
2. **Branch from `main`** using `<type>/<issue-number>-<short-description>`, for example `feat/31-rider-earnings` or `fix/42-otp-resend`.
3. **Commit:**

   ```
   <type>(<scope>): <summary>
   ```

   Types: `feat`, `fix`, `chore`, `refactor`, `docs`, `style`, `test`.
   Example: `fix(send): keep destination when going back from summary`

4. **Keep pull requests focused.** One issue per PR.

## Before opening a pull request

- [ ] `npm run typecheck` passes
- [ ] The app starts and the flows you changed work on at least one platform (Android, iOS or web)
- [ ] No secrets, debug logging or unused files are included

Never commit `.env` or any real keys or credentials.

In the PR description:

- Link the issue (`Closes #<number>`)
- Summarise what changed and why
- Add screenshots for UI changes where necessary
- Note anything you deliberately left out or deferred

**At least one maintainer review is required before merging.**
