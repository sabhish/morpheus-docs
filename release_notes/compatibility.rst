.. _compatibility:

************************
|morphver| Compatibility
************************

When installing and upgrading to |morpheus| |morphver|, refer to the following to ensure compatibility.

|morpheus| Application OS
=========================

The Morpheus Applications can be installed on the following Operating System versions:

+--------+--------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| OS     | Version(s)   | Notes                                                                                                                                                                                             |
+========+==============+===================================================================================================================================================================================================+
| CentOS | 7.x          | CentOS 8 for Appliance Hosts is scheduled for v4.2.1. v4.2.0 adds support for Morpheus Agent on CentOS 8.                                                                                         |
+--------+--------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Ubuntu | 16.04, 18.04 | FreeRDP 2.0 is not compatible with 16.04. Guacd will remain at 1.0.0 for Appliances running on 16.04, and is upgraded to 1.1.0 on Appliances running on 18.04.                                    |
+--------+--------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Debian | 8, 9         | FreeRDP 2.0 is not compatible with Debian 8. Guacd will remain at 1.0.0 for Appliances running on 8, and is upgraded to 1.1.0 on Appliances running on 9.                                         |
+--------+--------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| RHEL   | 7.x          | RHEL 8 for Appliance Hosts is scheduled for v4.2.1. v4.2.0 adds support for Morpheus Agent on RHEL 8.                                                                                             |
+--------+--------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Services
========

When externalizing MySQL, Elasticsearch and/or RabbitMQ services, the following versions are compatible with Morpheus |morphver|:

.. important:: Elasticsearch 7.x is required for |morphver|. Refer to :ref:`upgrading` section for more information.

+---------------------------------------+-----------------------+-------------------------------------+
| **Service**                           | **Compatible Branch** | **|morphver| Installer Version**    |
+---------------------------------------+-----------------------+-------------------------------------+
| MySQL                                 | 5.7                   | 5.7.29                              |
+---------------------------------------+-----------------------+-------------------------------------+
| Percona                               | 5.7, WSREP 31         | n/a                                 |
+---------------------------------------+-----------------------+-------------------------------------+
| Elasticsearch                         | 7.x                   | 7.6.0                               |
+---------------------------------------+-----------------------+-------------------------------------+
| RabbitMQ                              | 3.5-3.7               | 3.7.16                              |
+---------------------------------------+-----------------------+-------------------------------------+
| Redis                                 | REMOVED in v4.2.1     | REMOVED in v4.2.1                   |
+---------------------------------------+-----------------------+-------------------------------------+

Integrations
============

.. note:: Current iterations of Amazon AWS, Microsoft Azure, Google Cloud Platform, Digital Ocean, HPE OneView, OpenTelekom Cloud, IBM Bluemix, Softlayer and UpCloud are all supported.

+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Integration       | Supported Version(s)                                     | Known incompatibilities                                                                                                               |
+===================+==========================================================+=======================================================================================================================================+
| Ansible           | 2.7.x                                                    |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Ansible Tower     | 3.3.x                                                    |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| App Dynamics      | 4.5.x                                                    |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Azure Stack       | GA                                                       |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Cisco ACI         | 3.10                                                     |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Commvault         | v11 sp 12                                                |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Jenkins           | < 2.176.1                                                |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Kubernetes        | 1.x                                                      |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Kubernetes        | Major:"1", Minor:"14", GitVersion:"v1.14.1"              |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Microsoft Hyper-V | 2012R2, 2016, 2019                                       |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Nutanix AHV       | 5.0 - 5.10                                               | In 5.5 - 5.7 if Prism Central is managing Prism Element, image creation in Prism Element will function due to PC Image Management.    |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Openstack         | Juno, Kilo, Liberty, Mitaka, Newton, Ocata, Pike, Queens |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Rubrik            | 4.2                                                      |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| ServiceNow        | Kingston, London, Madrid, and New York                   |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Splunk            | 7.10                                                     |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Terraform         | v0.11.x                                                  | Not Compatible with v0.12.x (Support Planned)                                                                                         |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| vCloud Director   | 8.20, 9.1, 9.5                                           |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| Veeam             | 9.5u3, 9.5u4                                             |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| VMware ESXi       | 5.5, 6.0, 6.5, 6.7                                       |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| VMware Fusion     | 8, 9, 10+                                                |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| VMware NSX        | -V                                                       | NSX -T Support Planned                                                                                                                |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| VMware vCenter    | 5.5, 6.0, 6.5, 6.7                                       |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
| XenServer         | 7.x                                                      |                                                                                                                                       |
+-------------------+----------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+

.. note:: Non-listed versions may be compatible but are not verified.

If you have any specific requirements please contact support@morpheusdata.com
