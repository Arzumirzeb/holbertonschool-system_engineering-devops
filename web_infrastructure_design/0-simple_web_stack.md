# 0. Simple Web Stack


<p align="center"><img src="https://github.com/Arzumirzeb/holbertonschool-system_engineering-devops/blob/master/web_infrastructure_design/task_0.png"></p>

## Some specifics about this infrastructure:


### What is a server
A server is a computer program or device that provides a service to another computer program and its user, also known as the client. In a data center, the physical computer that a server program runs on is also frequently referred to as a server. That machine might be a dedicated server or it might be used for other purposes.
In the client/server programming model, a server program awaits and fulfills requests from client programs, which might be running in the same, or other computers. A given application in a computer might function as a client with requests for services from other programs and as a server of requests from other programs.
The term server can refer to a physical machine, a virtual machine or to software that is performing server services. The way that a server works varies considerably depending on how the word server is being used.

### What is the role of the domain name
Domain names serve as the navigational addresses of the internet, akin to street names, while IP addresses represent the actual locations. The Domain Name System (DNS) translates complex IP addresses into more memorable strings of letters, facilitating easier internet navigation. Organized hierarchically, domain names include top-level domains (TLDs), like .com and .org, and country code top-level domains (ccTLDs), such as .fr or .au. Subdomains further delineate the hierarchy, with second and third-level domains typically denoting organizations or specific servers within them. Domain names provide simple identification and are easily memorable compared to IP addresses, enhancing accessibility and usability on the internet.

### What type of DNS record www is in www.foobar.com
The "www" in "www.foobar.com" typically refers to a hostname and is associated with a DNS record known as a "CNAME" (Canonical Name) record. This CNAME record maps the hostname "www" to the domain name "foobar.com." It essentially acts as an alias, directing traffic intended for "www.foobar.com" to the same location as "foobar.com." This setup allows websites to be accessed using the common "www" prefix in the URL.

### What is the role of the web server
The end user processes a request via a web browser installed on a web server. The communication between a web server or browser and the end user takes place using Hypertext Transfer Protocol (HTTP). The primary role of a web server is to store, process, and deliver requested information or webpages to end users.

### What is the role of the application server
An application server acts as middleware between the operating system and various external resources, such as databases and internet services, and the users' applications. It hosts the user's business logic while ensuring accessibility and performance of the application. Despite challenges like variable client traffic and hardware failures, the application server ensures smooth functioning of the business application.

### What is the role of the database
In web application development, databases play a crucial role in storing and organizing data essential for the application's functionality. They serve as repositories for various information such as product details, customer information, and order history in systems like e-commerce websites. Developers rely on databases to store, retrieve, and modify data, making them indispensable components of web applications. Understanding databases is essential for comprehending the intricacies of web application development, as they facilitate seamless interaction between the application and its data.

### What is the server using to communicate with the computer of the user requesting the website
When a user requests a website, the server communicates with the user's computer using the Hypertext Transfer Protocol (HTTP) or its secure variant, HTTPS (HTTP Secure). These protocols define the rules for how information is exchanged between the server and the user's browser. The server processes the user's request and sends back the requested web page or resources, such as images or scripts, which are then rendered by the user's browser. This communication occurs over the internet, typically via TCP/IP (Transmission Control Protocol/Internet Protocol), allowing data to be transmitted reliably between the server and the user's computer.


## what the issues are with this infrastructure:


### SPOF
SPOF stands for "Single Point of Failure." It refers to a component within a system, such as a server, network device, or software module, that, if it fails, would cause the entire system to fail or become unavailable. In the context of IT infrastructure, identifying and mitigating single points of failure is crucial for ensuring high availability and reliability of systems and services. Redundancy, failover mechanisms, and disaster recovery plans are often implemented to address SPOFs and minimize their impact on operations.

### Downtime when maintenance needed
In manufacturing, “downtime” occurs when an unplanned event halts production for a period of time. This event can be a malfunction, repair, or changeover of tools or equipment. Maintenance downtime in particular is when a machine is not operating or being productive due to required maintenance work.

### Cannot scale if too much incoming traffic
Scaling your website allows you to accommodate increased traffic by adding additional computing resources to your hosting solution. Without adequate scaling, your website may experience performance issues or even crash under heavy loads, resulting in lost visitors, revenue, and damage to your reputation. By implementing scalability measures, you can ensure that your website remains responsive and reliable, even during periods of high traffic, safeguarding its performance and user experience.
