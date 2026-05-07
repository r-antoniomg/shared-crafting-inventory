---
title: About
layout: about
permalink: /about.html
# include CollectionBuilder info at bottom
credits: true
# featured-image value can be one objectid for a photo object in this collection, a relative path to an image in this project, or a full url to any image. If left blank, no featured image will appear at top of About page.
about-featured-image:
# set background-position for featured image, "center", "top", "bottom"
position: bottom
# major heading to display over featured image
heading: About the Collection
# paragraph text below heading in featured image
sub-heading: 
# additional padding added to the feature to increase size. Give value in em or px, e.g. "5em".
padding: 6em
# Edit the markdown on in this file to describe your collection
# Look in _includes/feature for options to easily add features to the page
---

## About this collection

This collection features images of crafting supplies (primarily wax stamps and wax seals) that are up for sharing among the owners of these supplies, as well as to plan purchases of new supplies by avoiding duplication.

In addition to the inventory and images, this site is meant to test various data and metadata best-practices and workflows.

## Guidelines

Work in progress. Last updated 2026-05-07

### Image guidelines

* Images should be taken or cropped to square (1:1) ratio
* Images uploaded to the objects folder should be a maximum of [FILE SIZE]
* Images uploaded to the objects folder should be [NUMBERS] pixels x [NUMBERS] pixels
* Images uploaded to the objects folder should be in [file extension] format
* Filename convention: `objectid_owner initials_imageDate`
* Example: `st0001_ae_2026-03-20`

### Metadata guidelines

* [REQUIRED BY CB] `objectid`: text string, alphanumericrd = parent record
  * `st` = stamp
  * `sl` = seal
  * `wx` = wax (beads or sticks)
  * `tl` = tool (spoon, spatula, mat, candle)
  * `####` = four-digit consecutive number (consecutive relative to full-inventory, not relative to specific alphabetical code)
  * Examples:
    * `st0001`
    * `wx0002`
    * `tl0003`
    * `tl0004`
   
* [REQUIRED BY CB] object_location : text string/objects/[filename].[extension]
* [REQUIRED BY CB] title : text stringIf available, use the product name from the vendor website as the title, in Sentence case
If not available, use a descriptive name in Sentence case
date : date in ISO-8601 formatDate product was acquired
If no exact date available use year only
owner_firstname : text string NOTE: EXPLORE CHANGING DEFAULT COLUMN NAME TO OWNEROwner of inventory item
If multiple owners of the same/similar item, separate by semi colon
item_type : 
manufacturer : text stringName of the company who manufactured the item, if known and/or the brand of the product
Example: Recollections
vendor : text stringName of the company from which the item was purchased
Example: Michael's
items_available : integer, no leading zeros NOTE: WHAT TO DO IF THE QUANTITY IS NOT CLEARLY DEFINED, SUCH AS WAX BEADS?how many of this item are available in totalExample: README stamp has two available items (2)
sharable : categoryyes
no
some : use this category if there are multiple items and only some are available for sharing
hobby_type : 
transportable : category yes
no
location : categoryinitials_house



CollectionBuilder-CSV is a "Stand Alone" template for creating digital collection and exhibit websites using Jekyll, given:

- a CSV of collection metadata
- a folder of images, PDFs, audio, or video files

Driven by your collection metadata, the template generates engaging visualizations to browse and explore your objects.
The resulting static site can be hosted on any basic web server.

[CollectionBuilder](https://github.com/CollectionBuilder/) is an set of open source tools for creating digital collection and exhibit websites that are driven by metadata and powered by modern static web technology.
See [CB Docs](https://collectionbuilder.github.io/cb-docs/) for detailed information.

{% include feature/image.html objectid="demo_001" width="75" %} 

<!-- IMPORTANT!!! DELETE this comment and the include below when you are finished editing this page for your collection. The include below introduces about page features. They will show up on your collection's about page until you delete it.  -->
{% include cb/about_the_about.md %} 
