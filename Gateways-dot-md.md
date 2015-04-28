# Gateways

## Basic setup
* MGCP
 * Initial setup.
```ios
    # config t
    # isdn switch-type primary-ni
    # clock participate wic 0
    # controller T1 0/0/0
    # pri-group timeslots 1-24, service type mgcp
    # no shut
    # int s0/0/0:23
    # isdn bind-l3 ccm
    # no shut
    # voice-port 0/0/0:23
    # no shut
```
* H323
 * 