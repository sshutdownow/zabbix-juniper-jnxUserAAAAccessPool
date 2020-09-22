# zabbix-juniper-jnxUserAAAAccessPool
ZBX-JUNIPER-jnxUserAAAAccessPool
==============

This template uses the SNMP to discover via LLD information about access pools inside routing instances on JunOS devices that are support JUNIPER-FIREWALL-MIB.


Items
-----

  * Discovery: jnxUserAAAAccessPoolOutOfMemory
  * Discovery: jnxUserAAAAccessPoolOutOfAddresses
  * Discovery: jnxUserAAAAccessPoolName
  * Discovery: jnxUserAAAAccessPoolInetNetwork
  * Discovery: jnxUserAAAAccessPoolAddressUsage
  * Discovery: jnxUserAAAAccessPoolAddressTotal
  * Discovery: jnxUserAAAAccessPoolAddressesInUse
  
Triggers
--------
  * Discovery: Address pool out of memory
  * Discovery: Address pool out of addresses
  * Discovery: Addresses exhausted for whole chain of pool(s)
  * Discovery: Addresses exhausted for pool
  
Graphs
------

  * Discovery: Pool Addresses Usage
  
Installation
------------

1. Import **zbx-Template jnxUserAAAAccessPool.xml** file into Zabbix.
2. Add to your host the **{$SNMP_COMMUNITY}** macro with your SNMP community as value.
3. Associate **Template jnxUserAAAAccessPool** template to the host.

Note
------------
There are two predefined pools called **_DAP** and **_DAPV6**. It seems that they are used for clients with static IP addresses (Framed-IP-Address).

### Requirements

This template was tested for Zabbix 4.4.0 and higher.There are no additional requirements.

### Copyright

  Copyright (c) 2020 Igor Popov

License
-------
   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.

### Authors

  Igor Popov
  (ipopovi |at| gmail |dot| com)
