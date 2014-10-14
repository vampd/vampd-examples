#Local Git Repo

Every now and then we run into a situation where we are not able to use a remote
git repo and when that time comes, we may have to pull down or initialize a repo
and make our commits locally and push them remotely with password prompts,
nightmare procedures and many, many tears.

We understand that. That is why it is possible to use local repos for this project
as well (we don't condone it, but we understand.)

For that, you will notice that the path is very similar to that of the database
file that we see in existing_site example. It is absolute at `/vagrant` and then relative to
where the project lives within you vampd repo.

###Tip
Make a folder in your vampd directory called `sites`. Then inside there create a
folder for each site you work on. For example: `colorado`. And then inside there,
you can create a `code` directory where the git repo lives and a `db` directory
for where the database dumps reside. Now your paths to the repos and the
databases are similar.
