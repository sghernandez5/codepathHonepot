# Honeypot Assignment

**Time spent:** **6** hours spent in total

**Objective:** Create a honeynet using MHN-Admin. Present your findings as if you were requested to give a brief report of the current state of Internet security. Assume that your audience is a current employer who is questioning why the company should allocate anymore resources to the IT security team.

### MHN-Admin Deployment (Required)

**Summary:** How did you deploy it? Did you use GCP, AWS, Azure, Vagrant, VirtualBox, etc.?


I used GCP to deploy my honeypot. I followed the instructions within the assignment and created an account through GCP and donwloaded GCP SDK on my ubuntu machine. 

<img src="https://user-images.githubusercontent.com/70529850/165026012-897e1532-7168-4614-bda9-c07be8d124c7.gif">


The gif below shows how I navigated through my MH-ADMIN, Honeypot1 and my local machine. 


<img src="https://user-images.githubusercontent.com/70529850/165026408-c1f06a78-64a8-4b29-a0fa-e9ec72183d42.gif">


### Dionaea Honeypot Deployment (Required)

**Summary:** Briefly in your own words, what does dionaea do?


Dioanaea is the honepot that I created, to capture any malicious traffic that it intercepts into its fake network. Below shows the the attacks it has encountered from other machines. 

<img src="https://user-images.githubusercontent.com/70529850/165026094-2ee659ae-d2d1-4438-9aa0-ae3a956dfa88.gif">

### Database Backup (Required) 

**Summary:** What is the RDBMS that MHN-Admin uses? What information does the exported JSON file record?

MHN-Admin uses mysql as its RDBMS. The json file captures the type of attacks dioaneaea had and other information such as:
  - the ip address of the machine
  - the destination 
  -  the oid
  
 A snippet of the information captured in the json file is shown below:


<img src="https://user-images.githubusercontent.com/70529850/165028415-c6a6e731-6cea-4641-900a-8b426d2f4e66.png">

Below are other stats for my single honepot. 

<img src="https://user-images.githubusercontent.com/70529850/165028936-04199eb7-c132-4de2-8615-f7f05dee7481.png">

## Notes

I had quite a few issues with GCP, at first it couldnt recognzie which project I was using and had to switch to the project with enabled billing information. 

I did have the ui of my MHN server crash for a bit, it wasnt displaying the attacks. 

