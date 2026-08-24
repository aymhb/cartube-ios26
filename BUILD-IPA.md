# Build the experimental IPA

1. Create a GitHub repository and upload this project so `CarTube.xcodeproj` is
   at the repository root.
2. Open the repository's **Actions** tab.
3. Select **Build experimental iOS 26 IPA** and choose **Run workflow**.
4. When the run finishes, download the `CarTube-iOS26-unsigned` artifact.
5. Extract the artifact and install the IPA with Sideloadly.

The workflow builds with Xcode 26 on the `macos-26` runner. Sideloadly must
re-sign the unsigned IPA. A successful installation does not guarantee CarPlay
will accept the app's private entitlements.
