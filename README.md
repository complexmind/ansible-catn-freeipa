CatN FreeIPA Ansible Playbooks - README
=======================================

+ Copyright (2012-2013):

> > Fubra Limited
> > Manor Coach House
> > Church Hill
> > Aldershot
> > Hampshire
> > GU12 4RQ
> > <http://www.catn.com>
> > <support@catn.com>


SOFTWARE LICENSE:
-----------------

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.

See LICENSE.TXT file for more information.


DESCRIPTION:
------------
This playbook installs a FreeIPA Server in a node. 
All the vars to edit are in /group_vars/all.yml

HOW TO USE:
-----------
Edit /group_vars/all.yml with your desired configuration. 
Edit /hosts with THE SAME ip address than the previous configuration file. 


TO DO:
------------
"Be sure to back up the CA certificate stored in /root/cacert.p12 This file is required to create replicas. The password for this file is the Directory Manager password"
-Keep working apache server

ASSUMPTIONS:
------------
-Network layer properly configured (eth0).
-Kerberos server installed and configured. 
-Other layers firewalls configured to allow al least HTTP/S, DNS, NTP,  Kerberos, LDAP/S and DOGTAG.
-Ssh connection to hosts. 
