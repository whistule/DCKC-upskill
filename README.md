# DCKC Course Guide

A guide for Drumchapel & Clydebank Kayak Club members on organising training courses and assessments - how the funding works, how to find providers, how to handle sign-ups, and how to communicate with the group.

**Live guide:** https://whistule.github.io/dckc-course-guide/ *(once GitHub Pages is enabled)*

## What this is

A single-file HTML guide that covers:

- How the funding works (Paddle Scotland subsidy, club top-up, member contributions)
- Day rates for PSL / SKL training and assessment
- How to find and approach providers
- The DCKC approved providers list
- Step-by-step course organisation
- Signing up and handling payment
- Communicating with the group before, during, and after
- Guinea pigs for leader assessments
- Course info page links (for candidates, trainees, and guinea pigs)

## Editing

The entire guide is in `index.html`. All CSS and content is in that one file - no build step, no dependencies.

### Small edits

The GitHub web editor is the easiest route:

1. Open `index.html` on github.com
2. Click the pencil icon (top right)
3. Edit the HTML directly
4. Scroll down and commit the change with a short message describing what you changed

### Larger edits

Clone the repo and work on it locally:

```bash
git clone https://github.com/whistule/dckc-course-guide.git
cd dckc-course-guide
# edit index.html in your editor of choice
git add index.html
git commit -m "Describe what you changed"
git push
```

Double-click `index.html` to preview changes in your browser before pushing.

## Updating the DCKC approved providers list

Find the section marked `<!-- PANEL 3: PROVIDERS -->` and look for `<div class="provider-grid">`. Each provider is a `<div class="provider-card">` block - copy an existing one and change the name, discipline, and tags.

## Updating course info page links

Find the section marked `<!-- PANEL 7: COURSE INFO PAGES -->`. Placeholder cards have `class="role-card placeholder"`; to convert one into a live link, change the outer div to an anchor tag:

```html
<a class="role-card" href="https://dckc.co.uk/your-new-page/" target="_blank" rel="noopener">
  <div class="role-card-label">For candidates</div>
  <div class="role-card-title">SKL Assessment - Info for Candidates</div>
  <div class="role-card-url">dckc.co.uk/your-new-page</div>
</a>
```

## Publishing changes

Once a change is committed to the `main` branch, GitHub Pages republishes the live guide within a minute or two.

## Who can edit

Anyone with write access to this repo. Contact the coaching coordinator or [repo owner] to be added.
