## Oxidized
Oxidized is a network device configuration backup tool. It's a RANCID replacement!

* Automatically adds/removes threads to meet configured retrieval interval
* Restful API to move node immediately to head-of-queue (GET/POST /node/next/[NODE])
* Syslog udp+file example to catch config change event (ios/junos) and trigger config fetch
 * Will signal ios/junos user who made change, which output modules can use (via POST)
 * The git output module uses this info - 'git blame' will for each line show who made the change and when
* Restful API to reload list of nodes (GET /reload)
* Restful API to fetch configurations (/node/fetch/[NODE] or /node/fetch/group/[NODE])
* Restful API to show list of nodes (GET /nodes)
* Restful API to show list of version for a node (/node/version[NODE]) and diffs


#### Changelog

##### v0.1.0
* Initial version, based on [Oxidized](https://github.com/ytti/oxidized)
