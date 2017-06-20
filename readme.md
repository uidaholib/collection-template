# jekyll gh-pages friendly build a digital collections site

set the `_config.yml` variables

at root are index and about that become the central portal for all collections.

metadata for individual digital collections is placed in `collections_info.csv` template.

metadata for items in a digital collection are in individual csv files in the `collection_metadata` directory.

to generate pages for a digital collection, copy the `template` directory in `_digital_collections`.
The directory name must be used in the `collections_info.csv` data "collection" field.
Delete the `.md` stub page types you do not want to generate for the collection.
Each stub template has settings for the page.
Place a csv with metadata about all items in the collection in the `_data/collection_metadata` directory (following the template).
The csv must be named the same as the collection directory.
