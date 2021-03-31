This is the repository for *French Rococo Ébénisterie in the J. Paul Getty Museum*, by Gillian Wilson and Arlen Heginbotham. This digital book was first published March 30, 2012, by the J. Paul Getty Museum. It is available online at [http://www.getty.edu/publications/rococo/](http://www.getty.edu/publications/rococo/) and may be downloaded free of charge in multiple formats.

## About the Book

This catalogue focuses on French ébénisterie furniture in the Rococo style dating from 1735 to 1760. These splendid objects directly reflect the tastes of the Museum’s founder, J. Paul Getty, who started collecting in this area in 1938 and continued until his death in 1976.

The Museum’s collection is particularly rich in examples created by the most talented cabinet masters then active in Paris, including Bernard II van Risenburgh (after 1696–ca. 1766), Jacques Dubois (1694–1763), and Jean-François Oeben (1721–1763). Working for members of the French royal family and aristocracy, these craftsmen excelled at producing veneered and marquetried pieces of furniture (tables, cabinets, and chests of drawers) fashionable for their lavish surfaces, refined gilt-bronze mounts, and elaborate design. These objects were renowned throughout Europe at a time when Paris was considered the capital of good taste.

The entry on each work comprises both a curatorial section, with description and commentary, and a conservation report, with construction diagrams. An introduction by Anne-Lise Desmas traces the collection’s acquisition history, and two technical essays by Arlen Heginbotham (with Jessica Chasen and Michael Schilling) present methodologies and findings on the analysis of gilt-bronze mounts and lacquer.

## Using this Repository

This is one in series of multiformat publications using [Quire](http://quire.getty.edu), Getty’s new publishing framework. Quire is currently in beta, with the goal of it being released as free and open source software in the future. In the meantime, users are encouraged to request access at http://bit.ly/quire-signup. This repository can also be run locally to build the online site (but not the PDF or ebook formats) with [Hugo](https://gohugo.io/), the [static site generator](https://www.smashingmagazine.com/2015/11/modern-static-website-generators-next-big-thing/) at the core of Quire.

We are dedicated to maintaining this publication for years to come at the permanent URL, [http://www.getty.edu/publications/rococo/](http://www.getty.edu/publications/rococo/), and in its various formats and incarnations. For any updates to the book, we will be following something between an app and traditional book publication model. Updates will only be made in regulated chunks as formal revisions and new editions and will always be thoroughly documented here in the repository, as well as in the revision history included with each of the book’s many formats.

The primary content pieces of the book can be found in the `data` and `content` directories. The master branch represents the current, published edition at all times, and the revisions branch, when present, will show changes currently under consideration. We invite you to submit suggestions or corrections via pull request on the revisions branch, by posting an issue, or by emailing us at [pubsinfo@getty.edu](mailto:pubsinfo@getty.edu).

## Development Notes

This project was last built with the following software versions:

- Quire 0.18.2
- Node 14.15.5 / npm 6.14.11
- Hugo 0.72
- PrinceXML 12.5
- Pandoc 2.10.1

While v0.18.2 of the core Quire Starter Theme was used, a number of customizations were made:

- Custom cover design and fonts to match J. Paul Getty Museum collection catalogues series design
- Additional identification options for contributors, ie., `role: conservator`
- [IIIF](https://iiif.io/) compatibility (ported in from an as-yet-to-be-released version of Quire)
- Added opbject info to the catalogue/contents grid page

Within the theme itself, changes were made to the `source/css/variables.scss` and `source/css/print.scss` files. Outside of the theme, customizations can be found in the project’s `layouts` directory, and in `static/css/custom.css`.

### Images Submodule

Many of figure images for *Rococo* are licensed from third parties for use exclusively in this publication. As such, they are kept in a separate, private repository, https://github.com/thegetty/rococo-images/, which is linked to this main publication repository as a submodule in `static/img/figures/`. When cloning this repo for further development, you’ll permissions for the private repository and will need to clone recursively in order to clone both the main repo and the submodule.

```
git clone --recursive https://github.com/thegetty/rococo.git
```

## License

© 2021 J. Paul Getty Trust

Unless otherwise indicated, the text and images of this work are licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License]((https://creativecommons.org/licenses/by-nc/4.0/)). Figs. 1, 2, 3, 1-6, 2-6, 2-11, 3-6, 3-16, 4-3, 4-8, 5-3, 5-11, 6-3, 6-4, 7-4, 7-5, 7-6, 8-8, 9-8, 10-5, 10-6, 10-8, 11-2, 11-3, 12-3, 14-3, 14-10, 14-11, 15-5, 15-6, 16-3, 16-4, 16-9, 17-1, 17-2, 18-6, 18-9, 19-4, 19-5, 21-3, and 21-4 are reproduced with the permission of the rights holders acknowledged in captions and are expressly excluded from the CC BY-NC license covering the rest of this publication. These images may not be reproduced, copied, transmitted, or manipulated without consent from the owners, who reserve all rights.
