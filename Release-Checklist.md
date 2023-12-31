- prepare
  - [ ] Complete [milestone items](https://github.com/prettier/prettier/milestones)
  - [ ] Run on other projects to check for regressions
  - [ ] Write release notes
    - use `node scripts/draft-blog-post.mjs` to generate a blog post draft (a file named <code>*YYYY*-*MM*-*DD*-*version*.md</code> in [`website/blog`](https://github.com/prettier/prettier/tree/master/website/blog)) from `changelog_unreleased`
    - [prs-merged-since](https://npm.im/prs-merged-since) ([readme](https://github.com/suchipi/prs-merged-since#prs-merged-since)) may be useful
- publish
  - [ ] Run [release script](https://github.com/prettier/prettier/tree/main/scripts/release)
- postpublish
  - [ ] Merge release notes
  - [ ] Wait for release notes to deploy
  - [ ] Clean `changelog_unreleased`
    - use `node scripts/clean-changelog-unreleased.mjs`
  - [ ] Tweet from [`@PrettierCode`](https://twitter.com/PrettierCode) account via TweetDeck
  - [ ] Close milestone
  - [ ] Send schema PR generated by `node scripts/generate-schema.mjs` to [SchemaStore](https://github.com/SchemaStore/schemastore/blob/master/src/schemas/json/prettierrc.json) if we added a new option.
  - [ ] Update the [release checklist](https://github.com/prettier/prettier/wiki/Release-Checklist) with possible changes

Then monitor [Twitter](https://twitter.com/search?q=%40PrettierCode&src=typed_query&f=live)/[GitHub](https://github.com/prettier/prettier/issues) for any immediate issues 😄