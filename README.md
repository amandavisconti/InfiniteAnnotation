# InfiniteAnnotation
Building a Drupal annotation solution from scratch.

# Installation!
*Notes*: In cases where installing a module results in multiple checkboxes added to the module admin page (e.g. installing the Views module adds checkboxes for Views and Views UI), I'll specify below if anything but the checkbox next to the name of the module needs to be checked.

Before installing the modules, create subfolders named "custom" and a "contrib" in your sites/all/modules folder; install any modules you get from Drupal.org (contributed modules) in "contrib", and any custom modules (modules whose code has been altered from what's on Drupal.org, or aren't even on Drupal.org) into the "custom" folder. This will help you keep track of modules where code has been altered, which is important as installing the latest update of a module can overwrite custom changes.

- Install and enable the latest versions of the following modules:
  - [jQuery Update](https://www.drupal.org/project/jquery_update)
  - [Views Expost](https://www.drupal.org/project/views_expost)
  - [Views](https://www.drupal.org/project/views)
    - Also enable "Views UI" from the Module page
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

- jQuery Update (admin/config/development/jquery_update)
  - Set "Default jQuery version" to 1.8
  - Performance > jQuery and jQuery UI CDN = none

- Theming
  - Sidebar region for view block
  
- Views (admin/structure/views)
  - Click the "import" link. (*Note*: Currently, Drupal requires you to be logged in as UID 1 to see and use the "import view" link. UID 1 means the user with the ID 1—that is, the first user on the site, created during the Drupal installation process.)
    - Name: annosidebar
    - Paste in the text found in this repo at AnnosidebarViewImport.txt

- Permissions (admin/people/permissions)
  - 
