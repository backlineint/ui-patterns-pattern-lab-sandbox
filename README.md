# UI Patterns Pattern Lab Sandbox

## Initial install

Install Lando: https://docs.devwithlando.io/installation/installing.html

From the root of this repository, run:

`lando start`

`lando composer install`

`lando drush si standard -y --db-url='mysql://drupal8:drupal8@database/drupal8' --site-name='UI Patterns Pattern Lab Sandbox' --account-name=admin --account-pass=admin`

If you do not plan on making changes to the module (you are testing or demoing 
for example,) you can install the latest dev version via composer.

`lando composer require drupal/ui_patterns_pattern_lab:dev-1.x`

If you are planning on contributing to the module, you should instead clone the 
git repository (https://github.com/backlineint/ui_patterns_pattern_lab) into 
web/modules/custom and then run the following command to enable it:

`lando drush en ui_patterns_pattern_lab`

The necessary dependencies should already exist from the composer file in the 
project root.

## Usage

web/themes/custom contains a number of themes that have been used for testing.  
The ui_patterns_pattern_lab_sandbox theme contains a number of example patterns
that function as a test suite. Feel free to also install the theme and/or pattern 
lab instance of your choice and test away.

## Links

Repository: https://github.com/backlineint/ui_patterns_pattern_lab
Drupal Project Page: https://www.drupal.org/project/ui_patterns_pattern_lab
Documentation: https://www.drupal.org/docs/8/modules/ui-patterns-pattern-lab