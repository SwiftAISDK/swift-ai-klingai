<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-klingai 1.1.4

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-klingai.git", from: "1.1.4")
```

Products: `SwiftAIKlingAI`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# Kling AI for Swift

`SwiftAIKlingAI` adds Kling AI to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/klingai` and supports video generation.

Provider guide with models, options, streaming and errors:

- [Kling AI](https://swiftaisdk.github.io/SwiftAISDK/providers/klingai/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAIKlingAI` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAIKlingAI

let provider = try AIProviders.klingAI(configuration: KlingAIProviderSettings())
```

By default the provider reads `KLINGAI_API_KEY`, `KLINGAI_ACCESS_KEY` and `KLINGAI_SECRET_KEY` from the environment; values set in `KlingAIProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-klingai` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
