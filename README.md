# Angavu Exec — installable app

Same pattern as Angavu POS and Angavu MES: a tiny launcher on
GitHub Pages that installs like a real app and opens the live
Exec app (its own standalone Apps Script project, same
spreadsheet as everything else).

## Before hosting
1. Add Exec_Standalone_Code.gs as Code.gs and ExecIndex.html to
   a NEW standalone Apps Script project (script.new — do not
   create this from inside the spreadsheet).
2. Run installExecSchema once.
3. Deploy -> New deployment -> Web app -> Execute as: Me ->
   Anyone with Google account -> Deploy. Copy the /exec URL.
4. Edit index.html here: replace
   PASTE-YOUR-STANDALONE-EXEC-EXEC-URL-HERE with that URL.

## Host on GitHub Pages (new repo, e.g. "angavu-exec")
1. github.com -> New repository -> angavu-exec -> Public -> Create
2. Upload these 6 files: index.html, manifest.json, sw.js,
   icon-192.png, icon-512.png, icon-512-maskable.png
   (upload the FILES themselves, not a folder containing them)
3. Settings -> Pages -> Branch: main, folder: / (root) -> Save
4. Confirm the live URL shown on that Settings->Pages screen.

## Install on devices
Android (Chrome): open the URL -> "Install app".
iPad/iPhone (Safari): Share -> Add to Home Screen.
