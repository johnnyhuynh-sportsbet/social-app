# Getting Started with Bluesky Social App

This guide provides a quick overview of how to set up and work with the Bluesky Social App codebase.

## Prerequisites

- Node.js 20+
- Yarn 1.22+
- For iOS development: macOS with Xcode
- For Android development: Android Studio with SDK

## Quick Start

### Web Development

```bash
# Install dependencies
yarn

# Start web app
yarn web
```

### Mobile Development

```bash
# Install dependencies
yarn

# Prepare native code
cp google-services.json.example google-services.json
npx expo prebuild

# Run on iOS
yarn ios

# Run on Android
yarn android
```

## Project Structure

- `/src` - Main application code
- `/modules` - Native modules
- `/assets` - Static assets
- `/docs` - Documentation
- `/bskyweb` - Go server for web app

## Common Tasks

### Running Tests

```bash
# Run unit tests
yarn test

# Run linting
yarn lint

# Run type checking
yarn typecheck
```

### Internationalization

```bash
# Extract and compile translations
yarn intl:build
```

### Building for Production

```bash
# Build web app
yarn build-web

# Build iOS app
yarn build-ios

# Build Android app
yarn build-android
```

## Debugging

- Web: Use browser developer tools
- iOS/Android: Access Developer Menu by shaking device or using keyboard shortcuts
  - iOS Simulator: Press Ctrl + Cmd ⌘ + z
  - Android Emulator: Press Cmd ⌘ + m or Ctrl + m

## Additional Resources

- [Build Instructions](./build.md)
- [Testing Documentation](./testing.md)
- [AT Protocol Documentation](https://atproto.com/guides/overview)
