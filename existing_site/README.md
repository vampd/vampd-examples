#Existing Site

This folder represents a json strucutred slightly for an existing site. You'll
notice how there is no repository in place except the default drupal repo. That
is because this existing site, is built straight off core.

While we know that never happens, this file is to demonstrate how a database file
is called from the json. When you run vampd, the whole vampd directory is available
at /vagrant during the vagrant provision. This means that when the mysql import
is happening it is looking for a file at `/vagrant/chef/roles/existing_site/existing_site.sql`.
Which can be found at `chef/roles/existing_site/existing_site.sql` in the vampd directory.

You'll also note that we are running deploy, import and update as the flags. This
is so that after we deploy our code, we are importing a database and then running
update.php.

This becomes highly powerful during a seamless deployment process because now
all updates to a site, besides content updates can be done through hook_update_N.
