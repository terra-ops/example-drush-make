# Drupal site ready for Terra

This is an example codebase for use with [Terra](http://github.com/terra-ops/terra-app).

When you add this site as an app, and create an environment, the build hooks will run, preparing the site codebase.

When you enable the environment, you can run the drupal install using drush:

```
terra app:add drupal https://github.com/jonpugh/drupal-terra
terra environment:add drupal local
terra environment:enable drupal local
drush @drupal.local site-install
```

You don't need to setup anything else.  The "build" hooks in terra handle writing the database credentials.
