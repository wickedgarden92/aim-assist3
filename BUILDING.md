# Build Predictive Input Buffer (.geode)

This source tree is configured to build on GitHub Actions using the workflow at `.github/workflows/build.yml`.

## Build on GitHub
1. Create a GitHub repository you own.
2. Upload the *contents* of this folder, including the hidden `.github` directory and `.github/workflows/build.yml`.
3. Commit the files to the default branch.
4. Open the repository's **Actions** tab and select **Build Geode Mod**. If it hasn't run yet, use **Run workflow** (or push a new commit).
5. Open the completed workflow run and download **Build Output** under **Artifacts**.
6. Extract the artifact and copy the `.geode` file to `Geometry Dash/geode/mods/`.

## Build locally
Install the Geode CLI and its SDK/binaries, then run in this folder:

```powershell
geode sdk install
geode sdk install-binaries
geode build
```

## Important limitations
- `mod.json` currently targets Windows Geometry Dash 2.2081 and Geode 5.11.2.
- The source README says the implementation has not been tested in-game. A successful compile does not prove input timing works correctly.
- The current mod ID/developer fields are placeholders (`tuusuario` / `TuUsuario`); replace them before publishing.
