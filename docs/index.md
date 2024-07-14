## Google Go Links (aka go/ links)
Google Go Links is an internal URL shortening and redirection system used within Google. It allows employees to create and share short, memorable links that redirect to longer URLs, making it easier to access frequently used resources, documents, and tools. The system is integrated into Google's internal network, enabling efficient navigation and collaboration among team members. Go Links can be customized, making it simple to create intuitive and context-specific shortcuts that enhance productivity and streamline workflows.

## EasyLinks (e2y.to) Links
e2y Links are my version of Go Links, created after I left Google following 15 years of service. Missing the convenience and efficiency of Go Links, I built e2y Links to replicate and expand upon the functionality of the system I relied on at Google.

Primarily focused on Google Workspace domains, e2y Links allows users to create their own short, memorable URLs for easy access to important resources. Data is isolated per domain to ensure security and privacy, but all access control needs to be handled in the target service.

Additionally, e2y Links are somewhat programmable, supporting regular expressions with group substitutions for more advanced and customizable use cases. They can also be hosted on a separate domain or subdomain, allowing use without the need for an e2y account, further enhancing flexibility and accessibility. (manual setup required).

```
Ex. 

name: ^/vin/(?P<VIN>[[:alnum:]]{17})$
destination: https://somedomain.com/path/*$VIN*

Will link e2y.to/vin/123456789abcdefgh to https://somedomain.com/somepath/*$VIN*
```
