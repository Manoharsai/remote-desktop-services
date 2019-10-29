# Remote Desktop Services
Blue Prism® is commonly installed and run on a virtualised infrastructure with virtual desktop images being used for Blue Prism Runtime Resources, and this remains the recommended deployment approach. However for users with specific IT infrastructure requirements, it may be desirable to deploy Blue Prism on a Remote Desktop Services (RDS) environment.

## About
Remote Desktop Services allows dozens or even hundreds of digital workers to be hosted on a single Windows Server, working simultaneously, without the need for a separate virtual infrastructure.


## Benefits
Using RDS to host Blue Prism can dramatically increase the number of virtual workers which can be deployed per server, as no additional overhead is required for the virtual infrastructure software or for the OS on each VDI. Additionally:

* Applications and OS updates are easier to manage, because they only have to be installed once per server, rather than on every VDI
* Adaptable scaling: dozens or even hundreds of workers can use the same server when the workload is light, or the number can be reduced when the workload is heavy

However it does have disadvantages, which are explored in more detail in the User Guide:

* High availability is difficult to achieve
* Sessions on a RDSH server all share a Windows process stack, slightly complicating process development
* Only supported on Windows Server, so digital workers cannot use a Windows Desktop environment
