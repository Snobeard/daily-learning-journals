# LJ Code 201 - Day 5
<a href="../README.md">`Home`</a>
<a href="201_README.md">`201 Index`</a>
<hr>

#### Images \- Inline Elements
  - <a src="https://www.gettyimages.com">gettyimages.com</a>
  - <a src="https://www.gimp.org">gimp.org</a>
  - <img title="<img title="hover text for image" />"" />

#### <u>JPG</u>
- #### Pros
  - Photos [for line art, logos, etc.]
- #### Cons
  - 'expensive' - bandwidth

#### <u>GIF</u>
- ###### Pros
  - good for [line art, logos, animation]
- ###### Cons
  - Not as good for photos - quality

#### <u>PNG</u>
- ###### Pros
  - photos
  - animation
  - transparency

---

# Color
- hex = #0F0F0F (rrggbb)

---

# Text
- ###### Serif
  - Has decorative flourish accents to text.
- ###### Sans Serif
  - Simpler layout.

---

# Git

- #### Git commandments
Always keep your local 'master' current with GH 'master':
     - ~git pull origin master (after every merge)

Always create new branches from 'master'
 - git checkout master
 - git pull origin master
 - git checkout -b <'new-branch'>

- #### Branching
Ways to work on different parts of the project and then merge to the master project.

    - Move to another branch: ~git checkout <'branch-name'>
    - Create new branch: ~git checkout -b <'branch-name'>
    - Push branch edits up: ~git push origin <'branch-name'>
    - Pull request: from <'branch-name'> to <'master'>

- #### Publishing shareable link as new branch
  ~git checkout -b gh-pages </br>
  ~git push origin gh-pages
