**This Arcance Template enables the deployment of FORGEJO and POSTRESQL services in the same container.**
➡️ It contains 2 separated networks : 
- public subnet 
- private subnet to grant access only to the database from the app itself, and this subnet is flagged as private thus the db port can't be accessed outside of the container

➡️ It also defines the right SVG icons automatically pulled from selfhst

➡️ Both services have healthchecks defined and operationals

➡️ If listening ports are not correctly defined in environment variables, default values are used.