# Google Cloud Workshop Notes 10/26/23

# Cloud Skills
- cloud certifications

# Website for Students - To Learn
- cloud.google.com/edu/students
- https://www.cloudskillsboost.google/games/4600

# Website for the workshop
- https://www.cloudskillsboost.google/games/4601
- access code: ch2-nm-campus-927

# Engineers
- Kevin: met a google recruiter at internship,  cat, parkour, works in security with cloud services like doordash etc
- Leslie Redd: works in a non-tech role, preached about how anyone can work in tech
- Naomi: works with fuscia on wifi requires OS's knowledge, learned about networking after changing teams
- Faharok: works with machine learning, gathering data for machine learning, ex: when google asks if two images are the same etc. captcha.
- Christian Michael: game host for cloud hero events, runs customer training for google cloud, hs experience: no sure, single mother 5 brothers, 1st gen, knew nobody in tech, got hispanic scholarship, mcnare scholars recipient for masters
- Mike: swe, worked with fucsia on wifi too from san jose
- Isabella: senior SWE, 9 yrs at google, came through campus recruiting, worked with ads before then went to search

# Takeaways
- everyone learned new things on the job, think about how to reinvent yourself and be open-minded to learning new things

# Hands-on labs
- 4 labs in 1st game
- ignore minutes
- can choose a fun name for the game
- may need to do some googling bc there might be some labs we won't cover for the competition
- we have 30 days access to do the missing lab to earn the skill badge and credentials

# Infrastructure Skills Overview
1. What is cloud computing? Think of it like running someone elses computer online, with servers
2. Can interact with google cloud in 4 ways
  - google cloud console: web user interfacr
  - google cloud sdk & cloud shell:cmd line interface
  - google cloud app: mobile app IOS & Android
  - REST-based API: a custom application interface
    
# Projects, roles & resource hiearchy
1. Organization
2. Project
3. Resources: app engine, cloud storage etc.
4. Below the resources there are **instances**
5. On the RHS we have policies like not everyone should have access to do everything

# Google Cloud Products
- products for computing

# Compute Engine
- offers managed virtual machines
- the cloud runs the vm's
- are created using google cloud console or the gcloud CLO

# Hosting resources
- google cloud has resources to host vm's in different regions + zones

# Google Cloud SDK + Cloud Shell
- cmd line version of google cloud
- allow u to manipulate things in google clouds like create vm
- cmd to to manipulate GSC : gsutil new bucket
- cloud shell provides no need for authorization

# What to do with cloud shell
- create, manage & connect to compute engine instances
- update firewall rules
- view system logs, ex: if there crashes

# What's a container?
- light-weight packages
- can containerize the langauge that are needed to run that particular program without overhead
- a constainer is a running instance of an image
- the package only runs those specifices dependencies needed
- container for front-end, one for back-end, etc.

# How do we organize these containers so they can interact?
- We use Kubernetes: a container orchestra

# Open-source Kubernetes (K8s/Kates)
- 100% open-source
- can fork and build on it

# Google Kubernetes Engine (GKE)
- quick to setup
- optimizes workloads, like when we want certain containers to work more etc.
- scales workloads
- kubetcl pronouced like ("cube-let") i think lol

# lab notes
- can redo up to 5 times, best score will count
- don't forget to click END lab
- make sure project number, 12-digit number matches

# zones
-Similarly, if you want to assign a static IP address to an instance, the instance must be in the same region as the static IP.

# cmds:
- gcloud auth list
- gcloud config list project
- gcloud config set compute/region europe-west1
- export REGION=europe-west1
- gcloud compute instances create --help
- gcloud compute instances list --filter="name=('gcelab2')"
- gcloud compute ssh gcelab2 --zone $ZONE
- sudo apt install -y nginx
