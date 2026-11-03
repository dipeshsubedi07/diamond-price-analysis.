# Data dictionary

Source: the accompanying coursework `metadata.pdf`. Column names are taken from the supplied CSV. The data contains 55,843 rows and ten columns.

| Column | Description |
| --- | --- |
| `carat` | Diamond weight in carats |
| `cut` | Cut category; the notebook accepts Fair, Good, Very Good, Premium and Ideal |
| `color` | Diamond colour category |
| `clarity` | Diamond clarity category; see source ambiguity below |
| `depth` | Depth value; the supplied metadata does not specify units or a formula |
| `table` | Value associated with the large, flat top facet; units are not specified in the metadata |
| `x` | Width, according to the supplied metadata |
| `y` | Length, according to the supplied metadata |
| `z` | Height, according to the supplied metadata |
| `price` | Price in USD |

## Source ambiguities

The source describes `clarity` as the diamond's “carat type”, which appears inconsistent with its column name and values such as SI1 and VS2. This dictionary identifies the apparent typo without claiming an authoritative correction. The source provides no explicit dimensional units, depth/table formulas, full category codebook, publisher or redistribution licence.

The raw data includes colour `Z`. Its validity is not established by the supplied metadata, and the notebook does not validate colour or clarity categories. It validates only `cut` categories.
