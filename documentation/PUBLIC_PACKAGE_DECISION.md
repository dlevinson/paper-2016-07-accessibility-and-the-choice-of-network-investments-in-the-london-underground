# Public Package Decision

Audit timestamp: 2026-05-17 21:12:09 Australia/Sydney.

The previous `DATA-CODE-ALREADY-UPLOADED` classification was too optimistic. Rereading the paper shows concrete source data and workflow dependencies beyond the article DOI: historical borough population data, Underground/surface rail network data, OpenStreetMap walking network background, manually digitized proposed lines, ArcGIS accessibility calculations, and an OpenTripPlanner historical GTFS comparison.

Local inspection found relevant London data and GIS source material. Those files are staged once in `../../../_shared_sources/london-historical-rail-accessibility` to avoid duplicating the same London coevolution inputs across several papers. This paper package keeps only the paper, the paper-specific derived OTP/headway workbook, and pointer documentation.

No respondent-level private data were identified in the staged public package. Drafts, correspondence, conference PDFs, article-source build clutter, generated figures, and large rendered images/movies were excluded.

Residual limitation: a full ArcGIS/OTP reproduction workspace was not found locally. If one later turns up, add it as code/workflow material; otherwise this package should be treated as the best available public source-data archive rather than a complete executable replication.
