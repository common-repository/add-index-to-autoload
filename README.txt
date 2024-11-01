﻿=== Add Index To Autoload ===
Contributors: raidboxes, mazeheld
Donate link: https://raidboxes.io
Tags: database, index. autoload, index-autoload, database speed
Requires at least: 4.1
Tested up to: 5.7
Stable tag: 1.1.1
License: GPLv3
Requires PHP: 5.6

Improve your WordPress-Website speed by adding an index to the autoload field of your WordPress database.

== Description ==

### Important: since WordPress 5.3, WordPress already has an index on the autoload field: https://core.trac.wordpress.org/ticket/24044
You don't need this plugin if you run WP >= 5.3

### Add Index To Autoload Plugin

This tool will speed up your database queries by adding an index to the “autoload” field.
With this index the query time for the autoload option will not increase with growing table size.
Therefore it helps speeding things up – especially with big option-tables.

### Plugin-Overview
This plugin offers four options:

* A one-click check mechanism to check if indexes on the autoload field exist
* An option that adds an index to the autoload field
* One-click index removal
* Adding a simple wp-cronjob, that periodically checks if the index still exists and notifies you, if it doesn’t.

### Support

If you encounter any issues, please leave a support ticket on the [WordPress.org Forum](https://wordpress.org/support/plugin/add-index-to-autoload)

### Bug reports

Bug reports for this Plugin are [welcomed on GitHub](https://github.com/MazeWebArchitect/add-index-to-autoload).
Please note GitHub is not a support forum, and issues that aren’t properly qualified as bugs will be closed.

== Installation ==

=== From within WordPress ===

1. Visit 'Plugins > Add New'
1. Search for 'Add Index To Autoload'
1. Activate Add Index To Autoload from your Plugins page.
1. Go to "after activation" below.

=== Manually ===

1. Upload the `add-index-to-autoload` folder to the `/wp-content/plugins/` directory
1. Activate the Add Index To Autoload through the 'Plugins' menu in WordPress
1. Go to "after activation" below.

=== How to ===

1. After activation you should see a new subpage under Tools > Add Index To Autoload
2. Backup your WordPress database (optional but recommended!)
3. Go to the "Options" Section below and click the Add Index button
4. Click the Check button: You should see a success message after a couple of seconds.
4a. If you don’t, please issue a support ticket on the  [WordPress.org Forum](https://wordpress.org/support/plugin/add-index-to-autoload)
5. Specify a periodic check for the autoload field (optional but recommended!)

== Frequently Asked Questions ==

= Can this plugin break my database? =

We have tested this plugin on +10000 WordPress-sites and on none did this plugin break anything.
But, we still recommend to backup your WordPress website, before using it.

== Screenshots ==

1. Screenshot of the management page of the plugin.

== Changelog ==

= 1.1.1 =
* Update: Checked with WordPress 5.7

= 1.1 =
* Added a check if the WordPress version is >= 5.3 if so, display a notice, that this plugin is not needed.

= 1.0 =
* Initial release
