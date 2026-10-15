# Sparrow

Hyperlocal delivery and errand app. React Native, Expo, and Expo Router.

The API is a separate repository: [OperaCode/Sparrow-backend](https://github.com/OperaCode/Sparrow-backend).

## Project structure

```
app/            Screens and routes (file-based routing)
  (tabs)/       Customer bottom-tab screens
  (rider)/      Rider screens
  auth/         Phone, OTP and onboarding flow
  send/         Send-a-package flow
  errand/       Errand flow (food, groceries, custom requests)
  delivery/     Delivery detail
components/     Reusable UI components
contexts/       React context providers (auth, deliveries, drafts, cart, address book)
lib/            Non-UI logic: pricing, geo helpers, catalog and mock data
constants/      Design tokens (colors, spacing, typography, shadows)
types/          Shared TypeScript types
assets/         App icon and favicon
```

## Development

```bash
npm install
cp .env.example .env
npm run dev
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). The product spec is [PRD.md](PRD.md).
