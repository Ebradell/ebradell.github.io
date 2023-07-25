# Ebradell Wiki

This is a microsite for the world of Ebradell, containing docs on many topics from characters, geography, lore and more.

## Contibuting

These docs are purposefully controlled via Git to allow us to collaborate and expand the world the more we play.

Simply checkout the code:

```bash
git clone https://github.com/Ebradell/ebradell.github.io.git
```

Then create a branch named after your change:

```bash
git checkout -b add-torol-backstory
```

Then on this branch make whatever changes you want. Once you're done, add the files to git and commit the changes:

```bash
git add .
git commit -m "Added backstory for torol, and added some flavour to his home regionn"
```

Once this is commited it's time to push it up to GitHub so the rest of us can review and merge the change:

```bash
git push
# or if it's the first time you've pushed this branch
git push --set-upstream origin add-torol-backstory
```

You can now go into the GitHub UI and create a Pull Request, then post a link to this into the Discord channel for others to review.

## How does this actual work?

This microsite uses [GitHub Actions](https://github.com/features/actions) and [GitHub Pages](https://pages.github.com/) as some simple free-hosting. 

Once something gets committed into the `main` branch, GitHub triggers Actions that are defined in the repository, that build up some static assets which are then deployed onto a simple webserver.

The framework itself uses simple [markdown](https://www.markdownguide.org/) files for text editing, just like this readme!