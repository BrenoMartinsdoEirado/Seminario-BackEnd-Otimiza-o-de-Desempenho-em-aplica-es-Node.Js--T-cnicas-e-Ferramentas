# Welcome to Clinic!

Please take a second to read over this before opening an issue. Providing complete information upfront will help us address any issue (and ship new features!) faster.

We greatly appreciate bug fixes, documentation improvements and new features, however when contributing a new major feature, it is a good idea to idea to first open an issue, to make sure the feature it fits with the goal of the project, so we don't waste your or our time.

## Bug Reports

A perfect bug report would have the following:

1. Summary of the issue you are experiencing.
2. Details on what versions of node and clinic you have (`node -v` and `clinic -v`).
3. A simple repeatable test case for us to run. Please try to run through it 2-3 times to ensure it is completely repeatable.

We would like to avoid issues that require a follow up questions to identify the bug. These follow ups are difficult to do unless we have a repeatable test case.

In addition, it is helpful if you upload your clinic data to help us diagnose your issues.
Use the `clinic upload` tool to do this:

```
clinic upload 10000.clinic-doctor
```

After the upload has finished, add the printed upload id to your issue.

## For Developers

All contributions should fit the [standard](https://github.com/standard/standard) linter, and pass the tests.
You can test this by running:

```
npm test
```

In addition, make sure to add tests for any new features.
You can test the test coverage by running:

```
npm run ci-cov
```

## For Collaborators

Make sure to get a `:thumbsup:`, `+1` or `LGTM` from another collaborator before merging a PR. If you aren't sure if a release should happen, open an issue.

Release process:

- `npm test`
- `npm version <major|minor|patch>`
- `git push && git push --tags`
- `npm publish`

-----------------------------------------

<a id="developers-certificate-of-origin"></a>
## Developer's Certificate of Origin 1.1

By making a contribution to this project, I certify that:

* (a) The contribution was created in whole or in part by me and I
  have the right to submit it under the open source license
  indicated in the file; or

* (b) The contribution is based upon previous work that, to the best
  of my knowledge, is covered under an appropriate open source
  license and I have the right under that license to submit that
  work with modifications, whether created in whole or in part
  by me, under the same open source license (unless I am
  permitted to submit under a different license), as indicated
  in the file; or

* (c) The contribution was provided directly to me by some other
  person who certified (a), (b) or (c) and I have not modified
  it.

* (d) I understand and agree that this project and the contribution
  are public and that a record of the contribution (including all
  personal information I submit with it, including my sign-off) is
  maintained indefinitely and may be redistributed consistent with
  this project or the open source license(s) involved.
