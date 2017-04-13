Alpha Pagination
=============
This module should be considered "BETA".

This module is an enhanced version of the standard "alpha pagination" module found at [Views Alpha Pagination](https://www.drupal.org/project/alpha_pagination) by Michael Bagnall (ElusiveMind).

If your site already has that module installed to provide alpha pagination for standard drupal views that are based entirely off of standard Drupal views data, this module can be a drop-in replacement for that module (just be sure to run update.php after checking out this code).

The extended feature allows this module to support views that are set to use Islandora Solr views.

## Usage
This pagination control is not exactly the same as the normal drupal **PAGER** control that can be configured in the Views editor.  This control must be added as a **HEADER** or **FOOTER** elements which are rendered around the paged content.  The standard pager may be suppressed.

Even though the settings for the Alpha Pagination allow the user to select which *View field to paginate against*, the selection should be "title".

Additionally, a **CONTEXTUAL FILTER** must be added that corresponds to the Islandora Solr title field of your content.  The default settings for this field are good, but for **WHEN THE FILTER VALUE IS IN THE URL OR A DEFAULT IS PROVIDED** "Specify validation criteria" should be set.

## Special Notes
This module exhibits an issue with caching that has been very difficult to debug.  For some reason, a subset of the relevant letters are cached -- and manually clearing the cache for the site restores the full set of alphabetical links to the objects.

## Author / License

Written by Brian Gillingham for the [University of Pittsburgh](http://www.pitt.edu).  Copyright (c) University of Pittsburgh.

Released under a license of GPL v2 or later.
