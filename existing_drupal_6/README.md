#Existing Drupal 6 Site

This folder represents a json strucutred slightly for an existing site built in Drupal 6, deploying the site and importing its code from a remote repository and its database from a folder on the local vbox machine.

One way to use vampd is to create a separate branch for each site you're currently working on, allowing you to provision each site as needed instead of all of them at once. This 'Existing Drupal 6 Site' example stores the database in the virtual machine's /assets/existing_drupal_6 folder (ignored through vampd's .gitignore), keeping the database out of version control and allowing you to switch from one branch of vampd to another without impacting the sites' databases.