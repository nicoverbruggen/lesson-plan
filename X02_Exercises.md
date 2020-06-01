# Extra 2: Exercises

## Working on hotkeys

Try getting used to common hotkeys.

## Setting up browser-sync for easy exercises

1. Install chocolatey or brew (Google it)
2. Install nodejs (`choco install nodejs-lts` / `brew install nodejs`)
3. Install browser-sync globally (`npm install -g browser-sync`)

After this, `cd` into the correct directory, and run:

	browser-sync start --server --files "path"

So, for a specific folder structure, you can do:

	browser-sync start --server --files "src/css/*.css" "src/js/*.js" "index.html"