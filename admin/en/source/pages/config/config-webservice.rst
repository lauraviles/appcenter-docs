.. Copyright 2016-2019 FUJITSU LIMITED

.. _config-webservice:

Configuring the Web Service
---------------------------

Each UForge Web Service instance runs inside a Tomcat application server. The web service has the following basic configuration information that is stored in a central configuration file: ``uforge.conf``. The main configuration attributes for the web service are:

	* External hostname used for incoming user connections
	* External hostname for downloading images (this uses port ``80`` allowing all cloud platforms to be able to communicate with UForge for publishing images)
	* Internal IP address used to connect with the other UForge services
	* HTTP port (default: ``8080``)
	* HTTPS port (default: ``8443``)
	* Administration console port (default: ``4848``)
	* Administration console credential information (user and password)
	* Root context of the web service (for example ``/uforge``)

When installing UForge via the deployment wizard some of the configuration attributes can be decided by the administrator. The deployment wizard also creates the uforge.conf file with all the configuration information.  

To view the uforge.conf file:

	1. Log in to the web service node as root::

		$ ssh root@<ip address of the node>

	2. Open the uforge.conf file::

		$ vi /etc/UShareSoft/uforge/uforge.conf

	3. After making appropriate changes in these files, you should run the following command on all the nodes (if multi-node the following order should be respected: compute notes, db nodes, web service nodes)::

		$ /opt/UShareSoft/uforge/tools/update_scripts/uforge_update.sh


For more information on Tomcat, see `http://tomcat.apache.org <http://tomcat.apache.org>`_
