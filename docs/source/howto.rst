How to start
=====

Prerequisites
------------

In order to run correctly these playbooks you have to:

- Calibrate and Release GCM *Calibration,Remediation,Scan* JT for each OS /MW that you want to remediate
- Creation of the "tools" project and its JT on ansible tower (you have to create one project and one job template for each tricode on the Tower)


Remediation JOB Creation
------------

In order to start using the project you must run the job template that was created as written in the installation page.
You have to specify into the variable called *"lista_progetti"* a list of project that need to be created on the ansible tricode
At the moment of writing these projects can be specificated:

 - SSH-UNIX
 - SUDO-UNIX
 - ITM-UNIX
 - ITM-Windows
 - HTTP-UNIX

There are 2 ways to specify this variable, one is from "extra variables" field. for example:

  .. image:: ansaibol-extravariables.png
  
Or you can create a survey like this:

  .. image:: survei.png
