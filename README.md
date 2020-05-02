# CIF-V4-PALO
API for CIFv4 that gives an API interfave for Dynamic Block Lists on Palo Alto

## Check Out the Feature Yourself To Install Follow The Instructions
Checkout our [cif-install-walkthrough.md](https://github.com/Jacksonurrutia/CIF-V4-PALO/blob/master/cif-install-walkthrough.md) where we talk through, step-by-step, how to setup CIF version 4, and how to plug in our feature. Setup will take you less than one hour.

## Once Installed Tests Can Be Performed On The Endpoint [Palo Endpoint](https://github.com/Jacksonurrutia/CIF-V4-PALO/blob/master/test-file/test_basics.py)

## More Information About the project

# NU CIF Capstone 
A Capstone project at the University of Nebraska-Omaha.  

We aspire to extend the functionality of [CIF version 4](https://github.com/csirtgadgets/verbose-robot/wiki/Introduction), a Cyber Threat Intelligence Management System, by adding an additional endpoint specific for Palo Alto firewalls.

## Highlights of Palo Alto Endpoint Extension
#### Compliant to Palo Alto 
* Palo Alto External Block List requirements described [here](https://docs.paloaltonetworks.com/pan-os/8-1/pan-os-admin/policy/use-an-external-dynamic-list-in-policy/external-dynamic-list.html#idf36cb80a-77f1-4d17-9c4b-7efe9fe426af), as well as [here](https://knowledgebase.paloaltonetworks.com/KCSArticleDetail?id=kA10g000000ClVYCA0).
#### Paging
* Palo Alto External Block List requirements specify limit of 5,000 IP addresses per block list.
      
      # Example usage
      # Returns first set of 5,000 IP addresses
      localhost:5000/palo/?page_num=1
      
      # Returns second set of 5,000 IP addresses
      localhost:5000/?page_num=2

#### User Input Sanitization 
* For security, user input is validated

