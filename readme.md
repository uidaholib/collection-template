# jekyll gh-pages friendly build a digital collections site

set the `_config.yml` variables

at root are index and about that become the central portal for all collections.

metadata for individual digital collections is placed in `collections_info.csv` template.

metadata for all items in all digital collections is placed in the `all_items.csv` template.

to generate pages for a digital collection, add a directory in `_digital_collections` following `template` example.
The directory name must be used in the csv data "collection" field.
Include a `.md` stub for each page time you want to create for the collection.
Each stub template has settings for the page type.
