# aws-scripts

This repo contains some scripts that will help you manage aws infrastructure. 


ami-copy-region 
===============
ami-copy-region is a bash script that uses aws cli tools to copy an ami and its tags to a new region.


Usage: 
./ami-copy-region --ami <ami> --source-region <region> --destination-region <region>

Example Usage: 
./ami-copy-region --ami ami-3cddfa43 --source-region us-east-1 --destination-region us-west-2



Prerequisites
-------------
* jq 
* aws cli tools 
* An AWS account
