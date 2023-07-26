# Reference Document
This document is intended for reference purposes. It contains a list of various tagging elements and their descriptions, with the aim of uniformity in tagging.

## Table of Contents
- Using the Undoubler
- Elements
    - [Div Elements]
    - [Head Elements]

## Using the Undoubler
In the repository you'll find a script titled 'undoubler'. This script was written to rectify some basic issues with the OCRed text, principally the use of double spaces in place of single spaces. The script is a Python script, and takes an input text ('raw_double.txt') and outputs it to a new clean file ('un_double.txt').

## Div Elements
```<div>``` (text division) contains a subdivision of the front, body, or back of a text. [4.1 Divisions of the Body](https://www.tei-c.org/release/doc/tei-p5-doc/en/html/DS.html#DSDIV)

The divider elements are numbered to provide a more immediate indication of their relative position in the hierarchy.

```<div1 type="issue" n="">``` elements are used as general containers for the entire issue (aka chapter) of the publication. This is mostly to future-proof the layout in case all the publications get combined into one file. The type is always "issue" and the n attribute is the issue number in modern Arabic numerals.

```<div2 type="{ forematter, section, endmatter }" n="">``` elements are used as general containers for the forematter, sections, and end of the publication issue. The forematter contains the title, epigraph, and catalogue data. The section contains the header and text. The endmatter contains the publication and printing notice appended to each issue. The type is always "forematter", "section", or "endmatter" and the n attribute is the section number in modern Arabic numerals when using the "section" divider.

## Head Elements
```<head type="" n="">``` (heading) contains any type of heading, for example the title of a section, or the heading of a list, glossary, manuscript description, etc. [4.2.1 Headings and Trailers](https://www.tei-c.org/release/doc/tei-p5-doc/en/html/DS.html#DSHD)

Types:
- title: The title of the document (ie. The Indicator)
- catalogue: Publication no., and date of publication (ie. No. XXIV.—WEDNESDAY, MARCH 22d, 1820.)
- header: The header of a section within the publication issue (ie. "ON THE REALITIES OF IMAGINATION.")