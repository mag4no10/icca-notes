# [+] Cloud Basics

## What is the Cloud

#### On-premises Information Systems Architecture 
- Workload                              (Everything we do)
- Services                              (DB services etc...)
- Virtual Machine                       (Operating systems..)
- Virtualization                        (Platform, Maintenance, Licencing)
- Physical Infrastructure               (Power, Network, Racks, Storage)
- Physical Facility                     (Cost of Space, Physical Security, Personnel)

#### Cloud Architecture
Same as above, that's the magic. Cloud manages the last 3 layers and let the client to use the other 3 \
cloud also has an extra optional layer between these two groups, the **Management Plane**.

#### Types of Cloud Services

- Workload ---> Software as a Service (SaaS)       hosting g-suite, microsoft 365
- Services ---> Platform as a Service (PaaS)       hosting web apps and db
- Virtual Machine ---> Infrastructure as a Service (IaaS) hosting a full vm

The line between them is blurred and not solid. \
The lower we go, the lower control we got. And the higher we go, the more ease of Administration we got.

- Through inet
- Through vpn tunnel
- Private circuit communication (expensive but safer)

## Who are the Cloud Providers

#### Cloud Market

Amazon is the biggest platform (45% of market share in 2019), Microsoft is the second (18% in 2019) and Google is the third
outside of China (5% in 2019).

#### AWS (Amazon Web Services)

Launched in 2006, over 190 countries, **over 175 products and services**, 18 global regions and over a million active users.

#### Azure (Microsoft Azure)

Publicly since 2010, 31 geographies, 57 regions, over 300k customers and **over 169 services**

#### GCP (Google Cloud Platform)

Launched in 2010, **over 90 services**, not sure how many users

#### Other Cloud Providers

- Around 20% market share
- Tencent and Alibaba in China (very present there)
- IBM and Oracle (pretty much same as the others)
- Digital Ocean
- Private cloud providers

## Why Choose the Cloud

#### Cloud Economics 
- Storage ---> Add more terabytes
- Compute ---> Add thousands of vm 
- Networking ---> Add more bandwith
  
Cloud is better because the client is being abstracted of the need to add more hardware or racks in the datacenter. The client can just invest in more storage or compute/networking.

#### CapEx vs OpEx

- On-premises capacity expansion = capital expense
    - Purchase equipment and licensing up-front
    - Depreciate and replace equipment
    - Renew licences
- Cloud-base capacity expansion = operational expense
    - Billed monthly for what is used
    - No equipment purchase
    - May or may not require licence purchase
- Capacity reduction
    - On-premises - posible sell excess equipment
    - Cloud - reduce monthly cost

#### Consumption-Based Spending
- Capacity-based spending
    - On-premises resources
    - Some cloud resources - virtual machines
- Consumption-based spending
    - Pay only for what is used
    - Functions. Lambda
    - Services
    - Storage

#### Functional Advantages
- Provision environments in minutes rather than days, weeks or months 
    - No capital equipment purchases
    - Streamlined provisioning process
- Built-in access and allocation management
- Reduced administrative overhead

#### Also, Maybe Not
- Existing investment
- On-going operational expenses
- Data fencing
- Regulatory compilance


# [+] Cloud Managment

## Managing Cloud Resources

#### Cloud Management Tools
- Web-based
- Command line (Linux-like(CLI) & Powershell-like)
- Rest API 

#### Web-based Cloud Management
- AWS (https://console.aws.amazon.com)
- Azure (https://portal.azure.com)
- GCP (https://console.cloud.google.com)
º
#### Command line Cloud Management
- AWS
    - AWS CLI (https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
    - AWS Powershell (https://docs.aws.amazon.com/powershell/latest/userguide/pstools-getting-set-up.html)
- Azure
    - Azure CLI (https://docs.microsoft.com/en-us/cli/azure/install/install-azure-cli) *
    - Azure Powershell ```Install-Module -Name Az -AllowClobber -Scope CurrentUser```
- Google Cloud
    - Google Cloud SDK
    - Component Management (kubectl)
    - Cloud tools for powershell (https://cloud.google.com/tools/powershell/docs/quickstart)
- Cloud Shell  

## Cloud Cost Management

#### Cloud Pricing Models
- Capacity (easier and you pay a fixed price)
- Consumption (harder, you pay what you use)
Beware of data transfer and transactional costs
#### Cloud Billing
- Billing Entity
- Billing Cycle
- Billing Management
- Billing Rate
- Marketplace Billing 
#### Cost Monitoring
- Budgets
- Alerts
- Monitoring Tools
- 3rd Party
#### Cost Optimization
- Agents
    - Azure Advisors
    - AWS costs anomaly detection
    - Google recommender
- Sizing
- Autoscale
- "Serverless" Options
- Long-term commitments