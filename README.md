# thepwagner

👋, I'm Pete (he/him).

My avatar is `pw` in [Open Sans Light](https://fonts.google.com/specimen/Open+Sans?preview.text_type=custom#standard-styles).
I like that it's identifiable across varying devices and abilities, and maintains my privacy.

## What I'm Hacking

### Automated dependency management

In projects stemming from https://github.com/thepwagner/action-update, I was experimenting with functionality similar to [Dependabot](https://github.com/dependabot/dependabot-core) as a stateless GitHub Action.

The [Renovate](https://github.com/renovatebot/renovate) project does 90% of what I need in this space, so I've switched to it!

### Git-backed CLIs

In projects like https://github.com/thepwagner/archivist and https://github.com/thepwagner/beancounter, I'm fiddling with CLIs that use a Git repository as their only data store.
For single-user apps this pattern is easy to deploy and maintain private federated data with optional synchronization (e.g. `archivist && git push`).
Git can provide viable [ACID](https://en.wikipedia.org/wiki/ACID) so these apps are forgiving to develop: you can see the diff a command had on the "database", and roll it back.

### Security

Across https://github.com/thepwagner/action-update there's themes of verifying dependency updates before proposing (e.g. GPG verification, Notary), and checksumming dependency updates once accepted.

In https://github.com/thepwagner/beancounter , I'm writing screen scrapers for banking sites. Commercial account aggregators often want your username/password, nope.
