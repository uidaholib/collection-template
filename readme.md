# jekyll gh-pages friendly build a digital collections site

> archived: this was a proof of concept for building digital collections using jekyll and metadata--see [CollectionBuilder](https://collectionbuilder.github.io/) for the eventual production project!

This is a prototype jekyll project used to build front end websites for digital collections.
Website generation is driven by collection metadata.
This basic prototype has data from the metadata exposed in the correct pages, but the visualizations and style are not built out.
It uses no plugins or dependencies, thus can be deployed on gh-pages (content is hosted else where).

The concept is that digital collection content is held in a repository such as CONTENTdm and quality metadata is developed.
The jekyll project uses the metadata to develop browsing and discovery visualizations on static web pages. 
Thus the front end of your digital collections are fast and responsive, while still providing easy access into the respository for more powerful search functions.
Invest time in improving metadata rather than customizing your repository or developing custom sites.

## Set up

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
