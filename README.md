# aws-scripts

This repo contains some scripts that will help you manage aws infrastructure. 


ami-copy
---------------

ami-copy-region is a bash script that uses aws cli tools to copy an ami and its tags to a new region.


Usage: 

./ami-copy --ami \<ami\> --source-region \<region\> --destination-region \<region\>


Example Usage: 

./ami-copy --ami ami-3cddfa43 --source-region us-east-1 --destination-region us-west-2



Prerequisites
-------------
* jq 
* aws cli tools 
* An AWS account

Bugs/Issues
-----------
* If you are running aws cli version aws-cli/1.11.136 and a copy takes more than 10min, you might get an error: "Waiter ImageAvailable failed: Max attempts exceeded"
* Use aws-cli tools version >= 1.14.53 
