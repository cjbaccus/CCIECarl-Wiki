# SIP specifics
The SIP protocol is a signaling protocol used with most modern Unified Communications devices.  Due to the simplicity and adversity of the protocol it is being adopted as the go to technology for most UC devices today.

## SIP basics
* Uses a markup language similar to HTML
* typically uses port 5060 and 5061 for secure
* Call flow diagrams can be easily made from SIP calls with basic tools in RTMT.
 * example:

{{{{{{ blue-modern
    SIPphone1->SIP-GW: send ringing
    SIP-GW->SIPphone1: send alerting
    SIPphone1->PSTN-Phone: ringing
    PSTN-Phone->SIPphone1: alerting
}}}}}}


@startuml
SIP2 -> SIPTrunk: Authentication Request
SIPTrunk --> SIP2: Authentication Response
@enduml


* debug messages
 * 200 ok
 * 401 error
