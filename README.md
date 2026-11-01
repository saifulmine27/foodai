# FoodLens BD - Android APK (GitHub diye)

1. GitHub-e notun repo banao.
2. Ei zip-er file gulo upload koro (package.json, capacitor.config.json, prepare.py, README.md).
3. Repo-te **Add file -> Create new file** -> naam dao: `.github/workflows/build-apk.yml`
   -> `build-apk.yml` file-er shob likha ekhane paste kore Commit koro.
4. **Actions** tab -> "Build Android APK" -> Run workflow (5-8 min).
5. Shesh hole **Artifacts -> FoodLens-BD-apk** download -> zip khule `app-debug.apk` install koro.

index.html upload korte hobe na: workflow nijei tomar site
(https://saifulmine27.github.io/fuuud/) theke niye nei.
Nijer index.html dite chaile root-e upload koro, oitai use hobe.

App khulle menu theke **Gemini API Key** chepe notun key boshao.

## API key APK-te age theke boshate chaile
Repo -> Settings -> Secrets and variables -> Actions -> New repository secret
Name: GEMINI_API_KEY   Value: tomar notun key
Tarpor Actions theke abar Run workflow koro. Key code-e lekha thakbe na.

## Notun UI (niche menu)
prepare.py ekhon phone-e niche bottom navigation (Home, Charts, Search, AI Scan, Dietitian) boshay.
Gear icon chaple Meal Log, Dark mode, Language, API Key ashe. Sudhu prepare.py replace kore Actions-e abar Run workflow koro.

## Notun version (charts timeframe wala)
Workflow prothome repo-r root-e `index.html` khuje; na pele live site theke nei.
Tai notun version GitHub Pages-e deploy kora thakte hobe, othoba `index.html` repo-r root-e upload koro.
prepare.py ekhon notun code-er key-o muche dey (key code-e thakle build bondho hoye jay).

## Update: index.html ekhon zip-er bhitore ache
Zip-er `index.html` = tomar latest version (charts period filter + % breakdown shoho), key shoriye deya.
Eta repo-te upload korle workflow live site na niye eta-i use korbe. Tai GitHub Pages update na korleo APK-te notun feature thakbe.
