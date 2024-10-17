# Expo Build Locally Github Actions

This repository contains examples of GitHub Actions workflows for building, testing, and submitting Expo applications locally.

## Workflows

### 1. Expo Build and Submit

This workflow allows you to build your Expo app for Android or iOS platforms and optionally submit it.

Key features:

- Configurable OS (Ubuntu or MacOS)
- Platform selection (Android or iOS)
- Build profile selection (development, preview, or production)
- Optional app submission

[View workflow file](expo-build-choice-and-submit.yml)

### 2. Build Preview APK for PR

This workflow automatically builds a preview APK when a pull request is opened, reopened, or synchronized.

Key features:

- Automatic version code calculation
- APK generation for preview builds
- Creation of GitHub releases
- Commenting on the PR with build information

[View workflow file](build-preview-apk-for-pr.yml)

### 3. Expo Build, Test, and Submit

This workflow builds the app, runs tests using Maestro, and can be configured to submit the app.

Key features:

- Builds on multiple API levels (21, 23, 29)
- Sets up Android emulator for testing
- Runs Maestro tests
- Configurable for different environments (QA, Production)

[View workflow file](expo-build-test-maestro.yml)

## Maestro Tests

The repository includes an example Maestro test file:

[View Maestro test file](maestro/test.yaml)

## Usage

To use these workflows in your project:

1. Copy the desired workflow files to your `.github/workflows/` directory.
2. Configure the necessary secrets in your GitHub repository settings.
3. Adjust the workflow files as needed for your specific project requirements.

Make sure to replace placeholder values and secrets with your actual project information.

## Requirements

- Expo project
- GitHub repository
- Necessary secrets configured in GitHub (EXPO_TOKEN, GOOGLE_SERVICES, etc.)

## Contributing

Contributions to improve these workflows are welcome. Please submit a pull request or open an issue to discuss proposed changes.

## License

[Add your license information here]
