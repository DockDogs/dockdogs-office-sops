DockDogs System Monitor & Status Page (Cachet)
===============================================


### What is Cachet?
_Cachet_ is an open-source _(free)_ service status page. 
* [Cachet Github Code Repository](https://github.com/CachetHQ/Cachet)
	* [Official Cachet Website](https://cachethq.io)

### How do I access the DockDogs Page?

* In your web browser visit [http://monitor.dockdogs.com](http://monitor.dockdogs.com)

### How do I administer the DockDogs page?


### Upgrading Cachet To New Version

* Open iTerm2 or Terminal.app
* $ `ssh 565f1c8189f5cf394700011d@health-dockdogs.rhcloud.com`
* $ `cd $OPENSHIFT_DATA_DIR`
* $ `cd bin`
* $ `./mgmutil` 
* $ `b` _(this is the option to upgrade)_
* Wait _(this may take a while)_
* Visit [http://monitor.dockdogs.com/dashboard](http://monitor.dockdogs.com/dashboard), login as an administrator and go to the **SETTINGS** page to confirm the new version has been installed.  