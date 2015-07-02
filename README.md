## Multi language setup, a Drush Make file ##

### Download ###

If your site folder:

- cd sites/all/modules
- git clone --depth=1 --branch 7.x-1.x http://git.drupal.org/sandbox/lolandese/xxxxxxx.git multilang_setup
- rm -rf !$/.git
- cd multilang_setup

More info at:
http://stackoverflow.com/a/11498124/523688


### Enable ###

With Drush 7.0 to build the profile, run:

drush make build-multilang_setup.make ~/www/spark --no-core --no-recursion

This will assemble all needed contrib.


### multilang_setup.info ###
Telling what core and contrib should be initially enabled.

#### multilang_setup.install ####
Setting up the rest, e.g.:
- Variable values.
- Text formats.
- Blocks.
- Entity (e.g. node) types (e.g. article, page).
- Taxonomy vocabularies.
- Fields.
- Roles.
- Permissions.
- Menus.
- Theme settings.


### More info ###

See https://drupal.org/developing/distributions.
