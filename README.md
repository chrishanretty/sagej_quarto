
# A Quarto extension for Sage Journals

## Creating a New Article

To create a new article using this format:

*TODO*: Replace the `<github-organization>` with your GitHub organization.

```bash
quarto use template <github-organization>/<%= filesafename %>
```

This will create a new directory with an example document that uses this format.

## Using with an Existing Document

To add this format to an existing document:

*TODO*: Replace the `<github-organization>` with your GitHub organization.

```bash
quarto add <github-organization>/<%= filesafename %>
```

Then, add the format to your document options:

```yaml
format:
  <%= filesafename %>-pdf: default
```    

## Options

The underlying [SAGE journal
class](https://uk.sagepub.com/sites/default/files/sage_latex_template_4.zip)
allows for several different options relating to paper size and
formatting style. The options for page size are:

 - `shortAfour` [210 x 280mm, 10pt, two-column]
 - `Afour`      [210 x 297mm, 10pt, , two-column]
 - `MCfour`     [189 x 246mm, 10pt, , two-column]
 - `PCfour`     [170 x 242mm, 10pt, , two-column]
 - `Royal`      [156 x 234mm, 10pt, single-column]
 - `Crown`      [7.25 x 9.5in, 10pt, single-column]
 - `Review`     [156 x 234mm, 12pt, single-column]

The options for bibliography are:

 - `sageh`   (SAGE Harvard style (author-year))
 - `sagev`   (SAGE Vancour style (superscript numbers)) 
 - `sageapa` (APA style (author-year))
 
 These are set through the `classoptions` key (`format` -> `sagej-pdf` ->`classoption`).
 

## Example

Here is the source code for a minimal sample document:
[template.qmd](template.qmd).

