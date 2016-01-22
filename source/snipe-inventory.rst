Snipe-IT Inventory Tracking
================================








Upgrading Snipe-IT To New Release Version
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Download release from Snipe-IT GitHub. ex:

::code-block:: sh
	:linenos:

$ curl -LOk https://github.com/snipe/snipe-it/archive/v2.0.6.zip
$ unzip v2.0.6.zip
# Update application folder (careful with the source directory trailing /!)
$ rsync -avut snipe-it-2.0.6/ /path/to/snipe-it
# Check directory permissions Complete this version's update steps. e.g.:
$ php composer.phar install
$ php composer.phar dump-autoload
$ php artisan migrate