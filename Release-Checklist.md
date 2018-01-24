1. Complete all [milestone items](https://github.com/prettier/prettier/milestones)
1. Run on other projects to check for regressions
1. Write release notes (Add a Markdown file named <code>*YYYY*-*MM*-*DD*-*version*.md</code> in [`website/blog`](https://github.com/prettier/prettier/tree/master/website/blog))
1. Merge release notes
1. Close milestone
1. Checkout `master`
1. Bump version in [`package.json`](https://github.com/prettier/prettier/blob/master/package.json)
1. Update [`CHANGELOG.md`](https://github.com/prettier/prettier/blob/master/CHANGELOG.md)
1. Run `yarn test_integration -u` to update snapshots (new parsers, `getSupportInfo`)
1. Commit
1. Run `yarn build`
1. Run `yarn test:dist`
1. `cd dist`
1. `npm publish`
1. `npm install prettier@latest`, do smoke tests on CLI and API
1. Push release commit
1. Create a [GitHub release](https://github.com/prettier/prettier/releases) to tag `master`
1. Wait for release notes to deploy
1. Check [blog](https://prettier.io/blog/) post
1. Tweet from [`@PrettierCode`](https://twitter.com/PrettierCode) account via TweetDeck
1. Create a new branch
1. Bump own `prettier` dependency (this will update the playground)
1. `yarn; yarn lint --fix; yarn lint-docs --fix`
1. Commit, PR, Merge

Then monitor Twitter/GitHub for any immediate issues 😄