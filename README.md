# InfiniteAnnotation
Building a Drupal annotation solution from scratch.

# Installation!

- Install and enable the latest versions of the following modules:
  - [jQuery Update](https://www.drupal.org/project/jquery_update)
  - [Views Expost](https://www.drupal.org/project/views_expost)
  - [Views](https://www.drupal.org/project/views)
    - Also enable "Views UI" from the Module page (it's included in the Views module install)
  - [Better Exposed Filters](https://www.drupal.org/project/better_exposed_filters)
  - [Ctools](https://www.drupal.org/project/ctools)
  
- Install and enable the following custom modules:
    - *Note*: the first two modules below are custom versions of these modules, *not* the modules you may find on Drupal.org
  - Annotation
  - Annotator
  - Highlighted_Annos
  
- Add the following to sites/all/libraries (create this libraries folder if it doesn't already exist):
  - Annotator
    - *Note*: this is a custom version of this folder found in this repo, *not* the library you may find on the AnnotatorJS website
    - Folder contains: annotator-full.min.js, annotator.min.css
    
# Configuration!

- Theming
  - Sidebar region for view block
  
- Annosidebar view import and configuration
