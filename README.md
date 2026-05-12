
# kernel-accessibility

<!-- badges: start -->
[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
[![](https://img.shields.io/badge/OSF-10.17605/OSF.IO/P5UFJ-1284C5.svg)](https://doi.org/10.17605/OSF.IO/P5UFJ)
[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-bd0000.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/license-CC_BY--NC--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
<!-- badges: end -->

<!-- Add DOI, [FAIR Software Checklist](https://fairsoftwarechecklist.net), [FAIR Software](https://fair-software.eu), and [Contributor Covenant badges](https://www.contributor-covenant.org) after publishing. -->

## Overview

This study aims to provide maps generated through the [Kernel Density Function](https://doc.arcgis.com/en/arcgis-online/analyze/kernel-density-global-function.htm) regarding access to healthy foods in favelas and urban communities, through the acquisition, processing, geocoding, and classification of [CNPJ](https://en.wikipedia.org/wiki/CNPJ) data obtained from the Brazilian Federal Revenue Service ([RFB](https://www.gov.br/receitafederal/)), as well as data on establishments classified as healthy food retailers from OpenStreetMap ([OSM](https://www.openstreetmap.org/#map=4/-15.13/-53.19)), from the [Overpass API](https://wiki.openstreetmap.org/wiki/Overpass_API).

The classification of food healthiness follows the [Locais-Nova](https://doi.org/10.1590/S2237-96222025v34.20240361.en) study, using Group 0 (G0). Although G0 is not part of the original classification, it is an existing subgroup within G1 + G2, composed of establishments that exclusively sell healthy foods which should constitute part of the population’s diet.

The report is available [here](https://cem-usp.github.io/kernel-accessibility/).

## Usage

The pipeline was developed using the [Quarto](https://quarto.org/) publishing system, along with the [R](https://www.r-project.org/) programming language. To ensure consistent results, the [`renv`](https://rstudio.github.io/renv/) package was used to manage and restore the R environment.

After installing the three dependencies mentioned above and setting all the keys, follow these steps to reproduce the analyses:

1. **Clone** this repository to your local machine.
2. **Open** the project in your preferred [IDE](https://en.wikipedia.org/wiki/Integrated_development_environment).
3. **Install package dependencies** by running [`renv::restore()`](https://rstudio.github.io/renv/reference/restore.html) in the R console. This will install all required software dependencies.
4. **Open** `index.qmd` and run the code as described in the report.

## Citation

To cite this work, please use the following format:

Pizzonia, M. A. Jr. (2026). *Mapping Healthy Food Accessibility in Brazilian Slums and Urban Communities* \[Computer software\]. Center for Metropolitan Studies, University of São Paulo. <https://cem-usp.github.io/kernel-accessibility/>

A BibTeX entry for LaTeX users is

```latex
@software{pizzonia2026,
  title = {Mapping Healthy Food Accessibility in Brazilian Slums and Urban Communities},
  author = {{Marcio Antonio Pizzonia Junior}},
  year = {2026},
  address = {São Paulo},
  institution = {Center for Metropolitan Studies, University of São Paulo},
  langid = {en},
  url = {https://cem-usp.github.io/kernel-accessibility/}
}
```

## License

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-bd0000.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/license-CC_BY--NC--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

> [!NOTE]
> The original data sources may be subject to their own licensing terms and conditions.

The code in this repository is licensed under the [GNU General Public License Version 3](https://www.gnu.org/licenses/gpl-3.0), while the report is available under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/) license.

``` text
Copyright (C) 2026 Center for Metropolitan Studies

The code in this report is free software: you can redistribute it and/or
modify it under the terms of the GNU General Public License as published by the
Free Software Foundation, either version 3 of the License, or (at your option)
any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with
this program. If not, see <https://www.gnu.org/licenses/>.
```

## Acknowledgments

<table>
  <tr>
    <td width="30%" align="center" valign="center">
        <a href="https://doi.org/10.17605/OSF.IO/ZE6WT"><img src="images/acessosan-logo.svg" width="140em"/></a>
    </td>
    <td width="70%" valign="center">
      This work is part of a research project by the Polytechnic School (<a href="https://www.poli.usp.br/">Poli</a>) at the University of São Paulo (<a href="https://usp.br/">USP</a>), in partnership with the National Secretariat for Food and Nutrition Security (<a href="https://www.gov.br/mds/pt-br/orgaos/SESAN">SESAN</a>) of the Brazilian Ministry of Social Development and Assistance, Family and Fight Against Hunger (<a href="https://www.gov.br/mds/">MDS</a>), titled: <em>AcessoSAN: Mapping Food Access to Support Public Policies on Food and Nutrition Security and Hunger Reduction in Brazilian Cities</em>.
    </td>
  </tr>
</table>

<table>
  <tr>
    <td width="30%" align="center" valign="center">
        <a href="https://centrodametropole.fflch.usp.br"><img src="images/cem-icon.svg" width="190em"/></a>
    </td>
    <td width="70%" valign="center">
      This work was developed with support from the Center for Metropolitan Studies (<a href="https://centrodametropole.fflch.usp.br">CEM</a>) based at the School of Philosophy, Letters and Human Sciences (<a href="https://www.fflch.usp.br/">FFLCH</a>) of the University of São Paulo (<a href="https://usp.br">USP</a>) and at the Brazilian Center for Analysis and Planning (<a href="https://cebrap.org.br/">CEBRAP</a>).
    </td>
  </tr>
</table>

<table>
  <tr>
    <td width="30%" align="center" valign="center">
      <a href="https://fapesp.br/"><img src="images/fapesp-logo.svg" width="160em"/></a>
    </td>
    <td width="70%" valign="center">
      This study was financed, in part, by the São Paulo Research Foundation (<a href="https://fapesp.br/">FAPESP</a>), Brazil. Process Number <a href="https://bv.fapesp.br/en/bolsas/231507/geospatial-data-science-applied-to-food-policies/">2025/17879-2</a>.
    </td>
  </tr>
</table>