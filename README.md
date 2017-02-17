# What is esportsinitiative.github.io?
The 5th iteration of ESI website. Main goals:

- [x] Static site hosted on GitHub Pages
- [x] Easy content creation and editing
- [x] Pages for:
  - [x] Events
  - [x] Sponsors
  - [x] Teams
  - [x] Games
  - [ ] Short Links

All easily solved and maintained by ***Jekyll!***


# Updating Events

*Notes*: Follows the example file in `_drafts/1995-01-01-template.md`

1. Create a new file in the folder `_events/`
2. Name the file `<date of event>-<name of event>.md` (e.g. `2016-09-01-smash-weekly.md` is the **Smash Weekly** on **Sept 1st, 2016**)
3. In the new file add the **metadata** and fill in the content:
 - Leave content which is **unknown** or **non-existent** blank
    ```yaml
    ---
    layout: "event"
    title:  "General Meeting"
    date:   2016-01-01 00:00:00
    date-end: 2016-01-01 00:00:00
    categories: "event"
    location: "Round Meeting Room"
    games:
    - "lol"
    tags:
    - "something"
    image-link: "/images/logos/esi/esi.png"
    event-link:
    ticket-link:
    rules-link: 
    description: "This is a general meeting"
    ---

    // Event info
    ```
4. Add event discription with links, images, text, headers, etc.
  - Markdown styling (symbolized by the `.md` extension) follows the following [syntax](https://guides.github.com/features/mastering-markdown/)


# Webmaster Stuff
## Setup
1. Pre-Setup
  - Are you on *Linux* or *OSX/MacOS*?
    - You have a good console! Proceed.
    - Optional [GitHub for Desktop](https://desktop.github.com/) 
  - Are you on *Windows*?
    - Download [Git](https://git-scm.com/) and [GitHub for Desktop](https://desktop.github.com/)
    - Git includes the amazing ***Git Bash*** console!
2. Install [Jekyll](https://jekyllrb.com/) (Notice this requires installing [Ruby](https://www.ruby-lang.org/en/) which on Windows needs to be installed with [RubyInstaller](https://rubyinstaller.org/))
3. Clone this repository into a good folder
  - Use: `git clone https://github.com/esportsinitiative/esportsinitiative.github.io.git`
  - **NOTICE**: If you installed [GitHub for Desktop](https://desktop.github.com/) you could clone through that for simplicity :)
4. Navigate to the project folder. (Command `pwd` should print something like `.../esportsinitiative.github.io/`)
5. Install the required gems: `bundle install`
6. Bring up the Jekyll site locally: `bundle exec jekyll serve`
7. Navigate to the site: `http://127.0.0.1:4000`

## Helpful Stuff:
It helped us! May it help you!

- [Jekyll](https://jekyllrb.com/)
- [Bootstrap](https://getbootstrap.com/css/)
- [Font Awesome Icons](http://fontawesome.io/icons/)
- [Sass Bootstrap](http://kvurd.com/blog/my-jekyll-blog-setup-bootstrap-sass-pygments/)
- [Flex Boxes <3](https://philipwalton.github.io/solved-by-flexbox/demos/vertical-centering/)
- [Jekyll Data Files](https://jekyllrb.com/docs/datafiles/)
- [Jekyll Collections](https://jekyllrb.com/docs/collections/)

Building stuff:

- [Jekyll Concat Strings](https://stackoverflow.com/questions/23688939/contatenate-append-a-string-to-another-one-in-jekyll-liquid)

## What isn't possible in Jekyll?

1. Use liquid in *.yaml* front matter (e.g. when creating posts) [discussed here](https://stackoverflow.com/questions/14487110/include-jekyll-liquid-template-data-in-a-yaml-variable)
