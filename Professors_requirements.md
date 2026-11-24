\#Automatic deployment of """containers"""

* Create an SDN network in Kathará with multiple switches
* Create a software that is capable of deploying services in the network	

  * Services are composed of multiple applications that communicate together to deliver the service (e.g., web server and database)
* Create a GUI (python or web) capable of:

  * Deploying service in the network (i.e., starting required applications on existing hosts)

    * Basic idea: choose host depending on usage (e.g., max 2 applications per host)
  * Choose communication requirements for applications

    * E.g., application A needs to communicate with application B
    * Upon choosing requirement, the software automatically configures flows in the switches (IPs and ports), keeping track of them, see next point
  * Stopping applications

    * Upon stopping, remove flows if not required anymore
* Show that applications can actually talk

  * Example of communicating applications are a web server and a database (create fake ones)

