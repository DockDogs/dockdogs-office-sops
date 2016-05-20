Snipe-IT Inventory Tracking
================================

Things, we have so very many things and must keep track of them. DockDogs uses `Snipe-IT <https://github.com/snipe/snipe-it>`_ to keep track of it all. This is a self-hosted `FOSS` platform that we host on ``lw.dockdogs.com.``


https://snipe-it-manual.readme.io/docs/getting-started



Upgrading Snipe-IT To New Release Version (OUTDATED)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Download release from `Snipe-IT GitHub Repo <https://github.com/snipe/snipe-it>`_ ex. ::


	$ curl -LOk https://github.com/snipe/snipe-it/archive/v2.0.6.zip
	$ unzip v2.0.6.zip

Update application folder (careful with the source directory trailing /!)::

	$ rsync -avut snipe-it-2.0.6/ /path/to/snipe-it
    
Check directory permissions Complete this version's update steps (example)::

	$ php composer.phar install
	$ php composer.phar dump-autoload
	$ php artisan migrate


