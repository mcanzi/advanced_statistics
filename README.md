# Advanced Statistics

Slides for *Advanced Statistics* (Dr Massimiliano Canzi, Department of Linguistics, University of Konstanz): a refresher of the Statistics course, generalised additive (mixed) models, random forests, power analysis by simulation, multivariate methods and, if time allows, figures for publication.

| | Session |
|---|---|
| 1 | Statistics refresher |
| 2 | Generalised additive models |
| 3 | Generalised additive mixed models |
| 4 | GAMMs in practice |
| 5 | Random forests |
| 6 | Random forests in practice |
| 7 | Power analysis |
| 8 | Factor analysis |
| 9 | Factor analysis in practice |
| 10 | Cluster analysis (in preparation) |
| 11 | Figures for publication (if time allows) |

The slides are online at [mcanzi.de/advanced_statistics](https://mcanzi.de/advanced_statistics/01_refresher.html).

## Rendering the slides

All data sets come from [{simling}](https://mcanzi.de/simling/), a package of simulated linguistic data whose help pages give the true model behind each data set: `lexical_decision_l2` (sessions 1 and 11), `price_f2` (2 and 3), `pupil_noise` (4), `td_deletion` (5), `accent` (6), `naming_pilot` (7), `language_attitudes` (8) and `web_registers` (9). `web_registers` is in the development version of {simling} on GitHub.

Knit `source/render_all.Rmd` to render every session into `docs`, which GitHub Pages serves. Knitting a single session also writes its HTML into `docs`. All sessions use the glacier theme of mcanzi.de (`source/theme-buttercup.css`): slate blue and ice, salmon accents, and glacier buttercups drawn in ink in the background. `source/slides_setup.R` sets the plot colours to match it. The fonts are in `source/fonts` and are embedded in each HTML file.

Requires `simling` (`remotes::install_github("mcanzi/simling")`), `tidyverse`, `revealjs`, `broom`, `lme4`, `lmerTest`, `patchwork`, `ggeffects`, `ggrepel`, `ggridges`, `mgcv`, `tidygam`, `itsadug`, `rpart`, `ranger`, `simr`, `psych`, `GPArotation` and `lavaan`; optional: `qrcode` (QR codes), `ragg` and `systemfonts` (Atkinson Hyperlegible in the figures).

## License

Course materials © Massimiliano Canzi, licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (see `LICENSE.md`). Code is licensed under the MIT License (see `LICENSE-CODE.md`). The fonts used in the slide theme (Atkinson Hyperlegible, Bricolage Grotesque, JetBrains Mono) are licensed under the SIL Open Font License 1.1 (see `source/fonts/OFL-*.txt`).
