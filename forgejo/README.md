**This Arcance Template enables the deployment of FORGEJO and POSTRESQL, RUNNER with DOCKER-IN-DOCKER services in the same container.**

➡️ The container contains 4 differents services.

➡️ It contains 2 separated networks : 

    ⭐ Public subnet shared by fogejo, the runner and docker-in-docker (192.168.254.8/29)

    ⭐ Private subnet to grant access only to the database from forgejo only, and this subnet is flagged as private thus the db port can't be accessed outside of the container (192.168.254.0/29)

    ⭐ All subnets are Class C and as they are using a /29 mask they only allow 6 hosts by subnet, I personally believe that it's more than necessary 😃

➡️ It also defines the right SVG icons automatically pulled from ([selfh.st](https://selfh.st/icons/)), for the forgejo it defines the same icon, and a different one for the database.

➡️ All services have healthchecks defined and fully operationals.

➡️ each container is relying on other dependencies.

➡️ If listening ports are not correctly defined in environment variables, default values are used.