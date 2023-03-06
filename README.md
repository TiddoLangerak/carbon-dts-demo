### Steps to reproduce
1. Clone this repo
2. `npm install`
3 `npx tsc --noEmit index.ts` - this errors

### Steps to validate the fix
1. Checkout the branch with the fix: https://github.com/TiddoLangerak/carbon/tree/fix/icon-unicode-typescript-export
2. In that branch, run `npm install && npm run build && npm run build:types && npm link`
3. Back in this repo, run `npm link carbon-react`
4. `npx tsc --noEmit index.ts` - no longer an error
5. Cleanup: `npm install`
