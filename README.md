# rfc-book

This is a repository that reads [polkadot-fellows RFCs](https://github.com/polkadot-fellows/RFCs/) and generates an online book.

## How it works

- First, we downloaded the RFCs contained in the RFCs repo - these are "approved" RFCs.
- Second, we download the RFCs contained in open PRS - those are "proposed" RFCs.
- We construct a web page using [mdBook](https://github.com/rust-lang/mdBook).
- Last, the web page is deployed to github pages under [github.com/paritytech/rfc-book](https://github.com/paritytech/rfc-book/).

### Update method

The book is updated on a cron-based manner, because watching every change in the repository (including pushes to PRs coming from forks) seems unfeasible.
