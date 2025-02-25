The files in this folder should in theory be generated after querying the
https://plugins.deckbrew.xyz/plugins endpoint on a schedule via github
actions.
- Get the latest commit hash of decky-plugin-database
- Compare hash against the previous hash saved in this repo
- If the hash is different, make a new branch on GH
  - Request data from https://plugins.deckbrew.xyz/plugins
  - Generate new metadata files for _store
  - Clean up any old metadata files, add new metadata files
  - Update commit hash
  - Make PR
  - Merge PR