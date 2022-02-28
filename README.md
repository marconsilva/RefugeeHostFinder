# RefugeeHostFinder
Open and public project to build a open and free Web Application to help Any Refugee from any conflict area in the world to find volunteer hosts around the world that they could contact and stay with during a crisis.

The goal is to create a cloud based, multi-language platform that both Hosts and Refugees could use to find safety in a crisis.

From a technical point of view the solution architecture should look something like the following image:
![alt text](https://raw.githubusercontent.com/marconsilva/RefugeeHostFinder/main/common/Architecture/refugeeHostFinder_Architecture.drawio.png "Architecture Diagram")

In detail the solution is composed of the following architecture blocks:
- A Web Site were the users could find all the information and the hosts would use as a BackOffice to manage their information as well
- A WebAPI with all the logic to serve the Website
- A Azure AD B2C that would work as a IdP for all the user's identities, with social media account integration and all the profile management capabitilites
- A Blob Storage account to handle all the images and unstructured information from the website
- A CosmosDB that would handle all the structured metadata information about places to stay, messages, etc...
- Cognitive Services for translation of the website into all supported languages and even to help with communications between host and refugee
- A Chatbot to help refugees with questions supported by a QnA Knowlege Base
