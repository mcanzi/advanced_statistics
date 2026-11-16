# Advanced Statistics

Slides for *Advanced Statistics* (Dr Massimiliano Canzi, Department of Linguistics, University of Konstanz): a refresher of the Statistics course, generalised additive (mixed) models, random forests, power analysis by simulation, factor and cluster analysis, and figures for publication.

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
| 10 | Cluster analysis |
| 11 | Cluster analysis in practice |
| 12 | Figures for publication |

The slides are online at [mcanzi.de/advanced_statistics](https://mcanzi.de/advanced_statistics/01_refresher.html). Participants install the course packages with [{konstats}](https://mcanzi.de/konstats/), which session 1 introduces together with {simling}.

## Tutorials

The hands-on sessions (4, 6, 9 and 11) come with a tutorial: the tasks of the slides as exercises, with an empty chunk for each answer, and a last section that goes beyond the slides. In class I use the slides; participants can work through the tutorial on their own. The sources, with solutions, are in `source/tutorials`. Knit `source/render_tutorials.Rmd` to check that every solution runs and to write the participants' sheets into `docs/tutorials`. The same sheets are in {konstats}, so `konstats::get_tutorial(4, ".", course = "advanced")` copies one into a project folder.

## Rendering the slides

All data sets come from [{simling}](https://mcanzi.de/simling/), a package of simulated linguistic data whose help pages give the true model behind each data set: `lexical_decision_l2` (sessions 1 and 12), `price_f2` (2 and 3), `pupil_noise` (4), `td_deletion` (5), `accent` (6), `naming_pilot` (7), `language_attitudes` (8), `web_registers` (9 and 11) and `korean_stops` (10). `web_registers` and `korean_stops` are in the development version of {simling} on GitHub.

Knit `source/render_all.Rmd` to render every session into `docs`, which GitHub Pages serves. Knitting a single session also writes its HTML into `docs`. All sessions use the glacier theme of mcanzi.de (`source/theme-buttercup.css`): slate blue and ice, salmon accents, and glacier buttercups drawn in ink in the background. `source/slides_setup.R` sets the plot colours to match it. The fonts are in `source/fonts` and are embedded in each HTML file.

Requires `konstats` and `simling` (`remotes::install_github("mcanzi/konstats")` installs both), `tidyverse`, `revealjs`, `broom`, `lme4`, `lmerTest`, `patchwork`, `ggeffects`, `ggrepel`, `ggridges`, `mgcv`, `tidygam`, `itsadug`, `rpart`, `ranger`, `simr`, `psych`, `GPArotation`, `lavaan` and `cluster`; optional: `qrcode` (QR codes), `ragg` and `systemfonts` (Atkinson Hyperlegible in the figures).

## License

Course materials © Massimiliano Canzi, licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (see `LICENSE.md`). Code is licensed under the MIT License (see `LICENSE-CODE.md`). The fonts used in the slide theme (Atkinson Hyperlegible, Bricolage Grotesque, JetBrains Mono) are licensed under the SIL Open Font License 1.1 (see `source/fonts/OFL-*.txt`).
