[puppet_url]: http://puppetlabs.com/

# puppet-modules

A collection of [puppet][puppet_url] modules. Some of which I wrote.

## Installation

You'll want to merge it with your system's `/etc/puppet/modules` directory. You can do this manually, or in git. The following command sequence should accomplish the latter option, but has not been tested:

1. `su root`
2. `cd /etc/puppet/modules`
3. `git init`
4. `git remote add AndersDJohnson git@github.com:AndersDJohnson/puppet-modules.git`
5. `git fetch AndersDJohnson`
6. `git merge --strategy ours --no-commit AndersDJohnson/master`
7. `git read-tree -m -u AndersDJohnson/master`

