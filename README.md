# Guardia

Mobile application built with Expo SDK 57, React Native, TypeScript, and Expo Router.

## Development

```sh
npm ci
npm start
```

Use `npm run android`, `npm run ios`, or `npm run web` to start for a specific platform. The iOS simulator requires macOS; use a physical device or an EAS development build when developing on Windows.

## Checks

```sh
npm run lint
npm run typecheck
```

## Structure

- `src/app/`: screens and the root navigation layout.
- `src/constants/`: shared light and dark theme colors.
- `src/hooks/`: theme selection and web hydration support.
- `assets/`: app icon and native splash assets, configured in `app.json`.

The app starts with a single Guardia screen. Add new screens under `src/app/` and keep non-route code outside that directory. Launcher and native splash assets are still the default artwork and should be replaced before release.

Install additional dependencies with `npx expo install <package>` to resolve SDK-compatible versions.
