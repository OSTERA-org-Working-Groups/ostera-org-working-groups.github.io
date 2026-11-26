# OSTERA Working Groups Website

This repository holds the source for [wg.ostera.org/](https://wg.ostera.org/), the home page of the OSTERA Working Groups site.

Each Working Group website is served from its own repository at `wg.ostera.org/<wg>/` (for example, [wg.ostera.org/jss/](https://wg.ostera.org/jss/)). This repository only holds the shared home page, the How to Participate page, the Public Reviews page, and the not found page.

## Adding a Working Group

To add a Working Group to these pages, add an entry to `docs/_data/working_groups.yml`. When its repository exists, set `repo` to `true`. When its website is live, set `website` to `true`; this also adds its Public Reviews to the Public Reviews page.

## Publishing GitHub Pages

GitHub Pages builds the `docs` folder of the `main` branch. Changes are live a minute or two after they are merged.

## Layout

| Path | Contents |
| --- | --- |
| `docs/_config.yml` | Site settings and the site navigation |
| `docs/_data/working_groups.yml` | The list of Working Groups shown on the home page and the Public Reviews page |
| `docs/index.md` | The home page |
| `docs/participate.md` | The How to Participate page, the one place that explains how to take part in the Working Groups |
| `docs/reviews.md` | The Public Reviews page, which lists every Public Review from every Working Group |
| `docs/404.md` | The not found page |
| `docs/CNAME` | The custom domain (wg.ostera.org). Do not delete it. |

The look and feel comes from the shared [OSTERA theme](https://github.com/OSTERA-org/ostera-pages-theme/).

<!-- BEGIN STANDARD TEXT -->

## Participating

Participation is open to OSTERA members. However, anyone may comment on a draft during its Public Review. See [How to Participate](https://wg.ostera.org/participate/), and read the [Contributing Guidelines](https://github.com/OSTERA-org-Working-Groups/.github/blob/main/CONTRIBUTING.md) before you open an issue or a pull request.

## Public Repositories

These repositories are public. Materials that are confidential to OSTERA members **MUST NOT** be stored in them, or anywhere else on GitHub. They **MUST** instead be stored in the [OSTERA Portal](https://member.ostera.org/).

## Publications

Approved documents are published at [pub.ostera.org](https://pub.ostera.org/), not in the Working Group repositories.

## Policies

The official OSTERA policies, including the IPR and Copyright Policy, the Working Methods, and the Code of Conduct, are published at [ostera.org/policies/](https://ostera.org/policies/).

## Intellectual Property

Anything you submit to OSTERA, such as an issue, a pull request, a comment, or an email, is a contribution under the [OSTERA IPR and Copyright Policy](https://ostera.org/policies/), and by submitting it you agree to that policy. Do not submit anything you do not have the right to contribute.

If you have knowledge of intellectual property rights, including patents, copyrights, trademarks, and service marks, for software or text, the use of which may be required to implement or publish any of the work items being considered, please disclose it by following the instructions at [ostera.org/ipr/](https://ostera.org/ipr/) or contact the Secretariat at [secretariat@ostera.org](mailto:secretariat@ostera.org).

## Code of Conduct

All participants are expected to follow the OSTERA [Code of Conduct](https://github.com/OSTERA-org-Working-Groups/.github/blob/main/CODE_OF_CONDUCT.md).

## Questions

For general questions about OSTERA, visit [OSTERA.org](https://ostera.org/) or contact the Secretariat at [secretariat@ostera.org](mailto:secretariat@ostera.org).

<!-- END STANDARD TEXT -->

## License

See [LICENSE.md](LICENSE.md).
