# Instructions on adding new data highlights

**Data highlights** is a section of the portal which contains news items promoting recent openly shared data that can potentially be used by many other researchers to make further discoveries or notable data re-use examples. This page contains instructions on adding new data highlights. Please see the instructions in the `README` file for information on contributing to the portal in general.

## Data highlight files

The data highlights are generated from Markdown formatted files contained in the `/content/english/highlights/` folder. The file name used here will also be the URL of the data highlight (e.g., `test-highlight.md` will become `https://covid19dataportal.se/highlights/test-highlight/`).

## Content of the data highlight files

Below is an example of a data highlight file content. You can copy this text into your markdown file and edit it to write your own data highlight.

```Markdown
---
title: Important new dataset shared
date: 2021-01-01
summary: A new dataset containing a large amount of valuable data has been openly shared.
banner: /highlights/banners/example.png
banner_large: /highlights/banners/example_large.png
banner_caption: "Illustration of X. The image was taken from Y."
---

This is the text of the highlight. This is the first paragraph. Introduce why this is an important topic.

This is the second paragraph of the text of the highlight. Markdown formatting should be used in the text. For example, you can make a piece of text italic by placing an asterisk at the beginning and end, *like this*. You can make a piece of text bold by placing two asterisks at the beginning and end, **like this**. You can also add a link with square brackets following round round brackets, [like this](https://example.com/data/).

This is the third paragraph of the data highlight.

*We typically put funder information near the end of the text, in italic font.*

#### Data

Here we describe exactly what data has been shared, how it can be re-used, and give links to where it can be downloaded.

#### Article

DOI: [_put_DOI_here](https://doi.org/_put_DOI_here)

Andersson, M., Johansson, S., Karlsson, A. Title of the journal publication *Journal Title*, **X** (X) (20XX).

```

On the top of the file, surrounded by `---`, basic information for this data highlight is provided. It contains the title; publication date (desired; Hugo needs to be run on that day or later for it to appear); summary text that appears in the homepage and in the main page of the Data highlights section; location of the illustration to be displayed on the homepage (`banner`); localtion of the illustration on the page of the highlight (`banner_large`); caption text that will appear under the illustration on the page of the highlight.

The title, date, summary, illustrations will appear where they are supposed to be.

## Illustrations

Typically, for each data highlight, we prepare two illustrations. One illustration is smaller and appears on the homepage of the portal as well as on the main page of the Data highlights section. The other illustration appears on the data highlight page itself.

The smaller illustration needs to have the width that is twice the length (i.e., length `300 px` and width `600 px`). This way, it will easily fit the look of the page layouts.

Both illustrations should be placed in the `/static/highlights/banners` folder. The URL of the images placed here will then be `https://covid19dataportal.se/highlights/banners/file_name.png`.

## Publishing

In order to publish a data highlight, make a pull request to the `develop` branch.
