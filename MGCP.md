[[_TOC_]]

# MGCP
The MGCP protocol for gateways is a master->slave relationship protocol.  The Cisco Communications Manager acts as the master and the gateway is the slave based on the commands the CUCM sends.

### MGCP Message types
* RQNT ~ Request 
* MDCN ~ Modify connection
* ...

### Troubleshooting
* no mgcp mgcp ~ to restart the protocol
* show ccm ~ to shee active registrations to CUCM
* show mgcp ~ to show mgcp status
* debugs
 * debug isdn q931 ~ shows active connections with called, calling, and disconnect cause codes.
 * debug isdn q921 ~ for l2 connection issues (usually PRI clocking or something like that)