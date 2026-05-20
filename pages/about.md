---
title: About
layout: about
permalink: /about.html
# include CollectionBuilder info at bottom
credits: true
# featured-image value can be one objectid for a photo object in this collection, a relative path to an image in this project, or a full url to any image. If left blank, no featured image will appear at top of About page.
about-featured-image: https://i.ibb.co/bfSj8sC/2026-05-16-crafting-banner-image.png
# set background-position for featured image, "center", "top", "bottom"
position: bottom
# major heading to display over featured image
heading: About this Collection
# paragraph text below heading in featured image
sub-heading: 
# additional padding added to the feature to increase size. Give value in em or px, e.g. "5em".
padding: 6em
# Edit the markdown on in this file to describe your collection
# Look in _includes/feature for options to easily add features to the page
---

This collection features images of crafting supplies (primarily wax stamps and wax seals) that are up for sharing among the owners of these supplies, as well as to plan purchases of new supplies by avoiding duplication.

In addition to the inventory and images, this site is meant to test various data and metadata best-practices and workflows.

The image used in the homepage banner and the About page banner was partly generated using the Jupyter notebook found in [https://github.com/r-antoniomg/image-tiles](https://github.com/r-antoniomg/image-tiles). Some additional edits were done manually.

## Guidelines

Work in progress. Last updated 2026-05-07

### Image guidelines

* Images should be taken or cropped to square (1:1) ratio
* Images uploaded to the objects folder should be a maximum of [FILE SIZE]
* Images uploaded to the objects folder should be in either `.jpg` o `.png` format
* Filename convention: `objectid_owner initials_imageDate`
  * Example: `st0001_ae_2026-03-20`

### Metadata guidelines

* [REQUIRED BY CB] `objectid`: text string, alphanumeric
  * `rd` = parent record
  * `st` = stamp
  * `sl` = seal
  * `wx` = wax (beads or sticks)
  * `tl` = tool (spoon, spatula, mat, candle)
  * `####` = four-digit consecutive number
    * NOTE: 'multiple' and 'compound' objects require a parent record and children records. In these instances, the consecutive number is assigned to the parent record and all children records will get the same consecutive number.
  * Examples:
    * `rd0001`
    * `st0001`
    * `sl0001`
   
* [REQUIRED BY CB] `object_location` : text string
  * `/objects/[filename].[extension]`
* [REQUIRED BY CB] title : text string
  * If available, use the product name from the vendor website as the title, in Sentence case
  * If not available, use a descriptive name in Sentence case
* `date` : date in ISO-8601 format
  * Date product was acquired
  * If no exact date available use year only
* `owner_firstname` : text string
  * If multiple owners of the same/similar item, separate by semi colon
* `item_type` :
* `manufacturer` : text string
  * Name of the company who manufactured the item, if known and/or the brand of the product
  * Example: Recollections
* `vendor` : text string
  * Name of the company from which the item was purchased
  * Example: Michael's
* `items_available` : integer, no leading zeros 
  * how many of this item are available in total
  * Example: README stamp has two available items (2)
* `sharable` : category
  * yes
  * no
  * some : use this category if there are multiple items and only some are available for sharing
* `hobby_type` : 
* `transportable` : category
  * yes
  * no
* `location` : category
  * initials_house
  * Example: ae_house