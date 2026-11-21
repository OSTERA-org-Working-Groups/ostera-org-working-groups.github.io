# OSTERA Working Groups Website

This repository holds the source for https://wg.ostera.org/, the home page of the OSTERA working groups.

Each working group website is served from its own repository at https://wg.ostera.org/&lt;wg&gt;/ (for example, https://wg.ostera.org/jss/). This repository only holds the shared home page, the participation page, and the not found page.

## Layout

| Path | Contents |
| --- | --- |
| `docs/_config.yml` | Site settings and the site navigation |
| `docs/_data/working_groups.yml` | The list of working groups shown on the home page |
| `docs/index.md` | The home page |
| `docs/participate.md` | The How to Participate page |
| `docs/404.md` | The not found page |
| `docs/CNAME` | The custom domain (wg.ostera.org). Do not delete it. |

The look and feel comes from the shared [OSTERA Pages Theme](https://github.com/OSTERA-org/ostera-pages-theme/).

## Adding a Working Group

Add an entry to `docs/_data/working_groups.yml`. When the group's website or repository goes live, set `website` or `repo` to `true`.

## Publishing

GitHub Pages builds the `docs` folder of the `main` branch. Changes are live a minute or two after they are merged.

## License

Contributions are made under the [OSTERA IPR and Copyright Policy](https://ostera.org/policies/).
