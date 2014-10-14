#Lightning

The lightning role installs the lightning profile and  exemplifies two
important things: install and make.

The roles allow for drupal to run a fresh install of any profile, for example lighting.
All that needs to happen is changing the profile under drupal->settings in the json.

More importantly though, this role utilizes the power of drush make and the vampd
eco system. Using vampd you are able to pull down a super light repo, and then
use drush make to make the site for you. This is how profiles are made on D.O.

You'll notice that in the JSON we specify which file to use for the make. You'll
also notice that `template` is set to `false` here. If `template` were set to `true`,
it would create a templated build.make template based on the information in your
json to pull your local/remote repository and the profile of your choice. This
is highly useful when using make as a team. To see what the template looks like
see [build.make.erb](https://github.com/vampd/drupal/blob/master/templates/default/build.make.erb)
