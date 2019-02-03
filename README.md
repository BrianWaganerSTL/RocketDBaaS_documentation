<h1>Rocket DBaaS</h1>


<h3>OverView</h3>

   The project is to create an Open Source DBaaS template that others could use



<h3>Technologies</h3>

  * Database: PostgreSQL 10
  
  * API: Django-Rest-Framework 2 (Python3.6)
  
  * UI: Angular 7
  
  * Minion: Django 2
  
  * LoadBalancing: HAProxy
  
  * Automation: Ansible
  
  
  
<h3>Rocket DBaaS Goals</h3>

  * API driven
  
  * Database backed
  
  * As easy to maintain, but flexible
  
  * Use OpenSource as much as possible
  
  
  
<h3>Rocket DBaaS MVP1</h3>

  * UI
  
    * Background refreshing
    
    * Overview page
    
      * Show all your clusters and servers
      
      * Show all active issues
      
      * Expandable Clusters to reveal the servers
      
      * Navigation to a given cluster's details
      
    * Cluster Details
    
      * Show Cluster and Servers details
      
      * Show tabs for Metrics (graphs), Backups, Restores, Activities, Issues, Contacts, Notes, (Logs not done)
      
    * Pool Servers
    
      * Display pool servers
      
      * Allows for faster builds, and needed in some companies to create clusters
      
    * Create Cluster
    
      * Fill in standard information
      
      * Fill in requested resource information, which will be used to pick the correct Pool Servers
      
      * Pick the servers from the PoolServers
      
      * Sumbit an API call to create
      
    * Reports
    
      * List Servers by DBMS <i>(Need to Code)</i>
      
      * List Contacts <i>(Need to Code)</i>
      
      * List Outages <i>(Need to Code)</i>
      
      * List Fail-Overs <i>(Need to Code)</i>
      
      * List Clusters/Servers that need to be OS and/or DB patched <i>(Need to Code)</i>
      
    * Admin Pages
    
      * Used to supplement UI
      
      * Uses Django-Rest-Framework API's
      
      * Provides direct access to all the underlying tables
      
        * You must really know what your doing to use this
      


<h2> Future Goals </h2>

* Patch Clusters in a Rolling fashion

    * Run against servers in a rolling manner
    
    * Update tables 
    
        * server is being patch
    
        * patch version
    
        * Patch Type (DB/OS)
    
        * Outcome
    
        * Store details of patch output

* Contacts for given Applications
    
    * Create/Update/Expire Contacts
    
    * Link Applications and 1 or more Contacts
    
    * Update Patching statuses to email Contacts

* A way to track activities that happen to a cluster (ie. Audit Log)
    
    * Examples: Failover, Down, Up, Patch, DbRestart, ServerRestart
    
    * For unplained events it would be nice to be able to put in a link to a ticket

* Store backup details

    * Store backups info like backupType, status, DbSizeGigs, BkupSizeGigs, start, stop
    
    * Roll them off when valid to do so

* Webpage for the intake form so we can use and reference it easier

* Produce a few reports or website, probably broken down by database type

    * Number of DBs
    
    * Size of DBs & trends
    
    * Size of Backups & trends
    
    * Unplaned Failovers
    
    * Downtime percents
    
    * Unpatched Servers/Clusters counts
    
    * Page showing costs per Application

* Allow users to

    * Have a dashboard of their databases
    
    * Allow them to sign up contacts
    
    * Create an Intake form to help set expectations
    
* Progress

    * To follow my progress and see the priority you can go to the following Kanban link
    
        [RocketDBaaS Status](https://github.com/BrianWaganerSTL/RocketDBaaS_documentation/projects/1)