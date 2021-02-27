# thepwagner

👋, I'm Pete. My pronouns are he/him.

My avatar is `pw` in [Open Sans Light](https://fonts.google.com/specimen/Open+Sans?preview.text_type=custom#standard-styles).

## What I'm Hacking

### Dependency update actions

In projects stemming from https://github.com/thepwagner/action-update, I'm experimenting with functionality similar to [Dependabot](https://github.com/thepwagner/action-update) or [Renovate](https://github.com/renovatebot/renovate) as a stateless GitHub Action.

### Git-backed CLIs

In projects like https://github.com/thepwagner/archivist and https://github.com/thepwagner/beancounter, I'm fiddling with CLIs that use a Git repository as their only data store.
For single-user apps this pattern is easy to deploy and maintain private federated data with optional synchronization (e.g. `archivist && git push`).
Git can provide viable [ACID](https://en.wikipedia.org/wiki/ACID) so these apps are forgiving to develop: you can see the diff a command had on the "database", and roll it back.

### Security

Across https://github.com/thepwagner/action-update there's themes of verifying dependency updates before proposing (e.g. GPG verification, Notary), and checksumming dependency updates once accepted.

In https://github.com/thepwagner/beancounter , I'm writing screen scrapers for banking sites. Commercial account aggregators often want your username/password, nope.
