# zhangyutiannan.github.io

Personal academic homepage of Yu Zhang (张宇), Dean of the Freedo AI Research Institute.

Live site: <https://zhangyutiannan.github.io/>

Built with [Jekyll](https://jekyllrb.com/), based on the [minimal-light](https://github.com/yaoyao-liu/minimal-light) theme by Yaoyao Liu.

### Using Locally with Jekyll

You need to install [Ruby](https://www.ruby-lang.org/en/) and [Jekyll](https://jekyllrb.com/) first.

Install and run:

```bash
bundle install
bundle exec jekyll server
```

View the live page at <http://localhost:4000>. The generated HTML files are in the `_site` folder.

### Editing Content

* Homepage intro: `index.md`
* Honors & awards / invited talks / contact: `_includes/awards.md`, `_includes/talks.md`, `_includes/contact.md`
* Publications: `_data/publications.yml` and `_data/preprints.yml` (teaser images in `assets/img/pubs/`)
* Services: `_includes/services.md`
* Site-wide settings (name, avatar, links): `_config.yml`

### Acknowledgements

This project uses the source code from the following repositories:

* [minimal-light](https://github.com/yaoyao-liu/minimal-light)
* [pages-themes/minimal](https://github.com/pages-themes/minimal)
* [orderedlist/minimal](https://github.com/orderedlist/minimal)
* [al-folio](https://github.com/alshedivat/al-folio)
* [AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io)
