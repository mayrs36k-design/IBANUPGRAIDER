# Run and deploy your IBAHUPGRAIDER app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio

## Run Locally

**Prerequisites:**  [Android Studio](https://android.com)

1. Open Android Studio
2. Select **Open** and choose the directory containing this project
3. **CRITICAL:** Locate the `App.zip` file in the root directory. Unzip it and place all extracted files directly into the project directory with your other files. The full source code could not be fully uploaded directly due to GitHub file size limits.
4. Allow Android Studio to fix any incompatibilities as it imports the project.
5. Create a file named `.env` in the project directory and set `GEMINI_API_KEY` in that file to your Gemini API key (see `.env.example` for an example)
6. Remove this line from the app's `build.gradle.kts` file: `signingConfig = signingConfigs.getByName("debugConfig")`
7. Run the app on an emulator or physical device
8. This app operates as a specialized "trash-drop" simulator game loop, handling real-time physics and object instantiation mapped directly via Gemini API context triggers.
