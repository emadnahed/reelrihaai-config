# reelrihaai-config

Public, signed data files for the ReelRihaai app. Nothing here is about any user.

- `signatures.json`: the detection-signature list the Android app downloads about once a day, so a screen
  that an app update broke can be fixed without an app release. It is signed (ECDSA P-256); the app
  ignores any file not signed with ReelRihaai's key, and the list can only name screens of apps
  ReelRihaai already supports. It is data only, never code.

Published with `scripts/sign-signatures.mjs` from the app repository.
