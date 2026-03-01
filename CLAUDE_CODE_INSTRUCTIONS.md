# Claude Code Instructions

Paste this prompt into Claude Code to deploy the project:

---

## Prompt to paste:

```
Create a new public GitHub repo called "tropical-carry-guide" and deploy it with GitHub Pages. Here's what to do:

1. Create the repo: `gh repo create tropical-carry-guide --public --clone`
2. Copy all files from this project folder into it (index.html, README.md, .gitignore)
3. Commit and push to main branch
4. Enable GitHub Pages on the main branch root: `gh api repos/{OWNER}/tropical-carry-guide/pages -X POST -f source.branch=main -f source.path=/`
5. Tell me the live URL when done
```

---

## Manual steps (if preferred):

```bash
# 1. Create repo
gh repo create tropical-carry-guide --public --clone
cd tropical-carry-guide

# 2. Copy files (adjust path to where you saved them)
cp ~/Downloads/index.html .
cp ~/Downloads/README.md .
cp ~/Downloads/.gitignore .

# 3. Push
git add .
git commit -m "🌴 Initial commit: Tropical Carry Guide"
git push origin main

# 4. Enable GitHub Pages
OWNER=$(gh api user --jq '.login')
gh api "repos/$OWNER/tropical-carry-guide/pages" \
  -X POST \
  -f source.branch=main \
  -f source.path=/

# 5. Get the URL
echo "https://$OWNER.github.io/tropical-carry-guide/"
```

The site should be live within 1-2 minutes at:
`https://{your-username}.github.io/tropical-carry-guide/`
