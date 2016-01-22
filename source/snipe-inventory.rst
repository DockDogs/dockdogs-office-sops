Snipe-IT Inventory Tracking
================================








Upgrading Snipe-IT To New Release Version
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Download release from `Snipe-IT GitHub Repo <https://github.com/snipe/snipe-it>`_ ex. ::


	$ curl -LOk https://github.com/snipe/snipe-it/archive/v2.0.6.zip
	$ unzip v2.0.6.zip
	# Update application folder (careful with the source directory trailing /!)
	$ rsync -avut snipe-it-2.0.6/ /path/to/snipe-it
	# Check directory permissions Complete this version's update steps. e.g.:
	$ php composer.phar install
	$ php composer.phar dump-autoload
	$ php artisan migrate


How do I change behavior for Read the Docs?
-------------------------------------------

When RTD builds your project, it sets the `READTHEDOCS` environment variable to the string `True`. So within your Sphinx ``conf.py`` file, you can vary the behavior based on this. For example::

    import os
    on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
    if on_rtd:
        html_theme = 'default'
    else:
        html_theme = 'nature'

The ``READTHEDOCS`` variable is also available in the Sphinx build environment, and will be set to ``True`` when building on RTD::

    {% if READTHEDOCS %}
    Woo
    {% endif %}