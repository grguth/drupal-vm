If you'd like to use the included configuration and Drush make file to install a Drupal 6 site using an older version of Drush (< 7.x), you may need to make some changes, namely:

  1. Drush < 7.x does not support .yml makefiles; if using Drush 5.x or 6.x, you will need to create the make file in the INI-style format.
  2. In your customized `config.yml` file, you will need to use the `default` installation profile instead of `standard` (for the `drupal_install_profile` variable).
  3. If the default drush-Drupal install fails due to PHP not allowing MySQL to be loaded, then in the customized`config.yml` file, you will need to specify `5.5` for the `php_version` variable.  
