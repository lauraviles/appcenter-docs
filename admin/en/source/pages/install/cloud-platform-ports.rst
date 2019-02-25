.. Copyright 2016-2019 FUJITSU LIMITED

.. _cloud-platform-default-ports:

Cloud Platform Default Ports
----------------------------

To allow UForge to register machine images, you must ensure that there is network connectivity to the cloud platforms you want to push the machine images to.  The table below provides the default port numbers of the cloud platforms supported, and indicates whether UForge uploads the machine image or requests the cloud platform to download.

.. warning:: For private cloud platforms, the port number may not be the default port number indicated.

+-----------------------+-----------+---------------------+------------------------+
| Cloud Platform        | Protocol  | Default Port Number | Method of Registration |
+=======================+===========+=====================+========================+
| AWS                   | TCP       | 443                 | UPLOAD                 |
+-----------------------+-----------+---------------------+------------------------+
| Azure                 | TCP       | 443                 | UPLOAD                 |
+-----------------------+-----------+---------------------+------------------------+
| CloudStack            | TCP       | 8080                | DOWNLOAD               |
+-----------------------+-----------+---------------------+------------------------+
| Google Compute Engine | TCP       | 443                 | UPLOAD                 |
+-----------------------+-----------+---------------------+------------------------+
| K5                    | TCP       | 443                 | UPLOAD                 |
+-----------------------+-----------+---------------------+------------------------+
| OpenStack             | TCP       | 9292 and 5000       | UPLOAD                 |
+-----------------------+-----------+---------------------+------------------------+
| Oracle Cloud          | TCP       | 443                 | UPLOAD                 |
+-----------------------+-----------+---------------------+------------------------+
| vCloud Director       | TCP       | 80 / 443            | UPLOAD                 |
+-----------------------+-----------+---------------------+------------------------+
| vCenter               | TCP       | 80 / 443            | UPLOAD                 |
+-----------------------+-----------+---------------------+------------------------+
