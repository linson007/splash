# Chat context screenshots

Review evidence for https://github.com/incoai/splash/issues/641.

These images render the actual SwiftUI composer from implementation commit `712cfbe85fb861bfe7f4649d30a1cf85385fd50a`.
The deterministic local test server uses a 1,024-token context and the fixture model `test-model`.
The ready state shows the same draft after starting a new chat; the full states keep the previous conversation, draft and attachment.

Generated with:

```sh
SPLASH_APP_SNAPSHOTS=/tmp/splash-context-review swift test --package-path app --filter ChatContextFlowTests
```

The screenshots are hosted on this evidence branch for embedding in the pull request.
