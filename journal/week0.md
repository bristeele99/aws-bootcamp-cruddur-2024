# Week 0 — Billing and Architecture

Here's the CD practice copying Andrew Brown's architecture

Didn't understand alot of the pictures, but learned enough about Lucid Chart to be dangerous.

<img src="/workspace/aws-bootcamp-cruddur-2024/journal/week0/Screenshot 2024-04-01 000532.png">

aws--cli-auto-prompt to enable auto complete
aws sts get-caller-identity (sanity check for who you are)

AWS REFERENCE CLI DOCUMENTATION VERSION 2 for commands

aws account get-contact-information
[gets my own account information]

[cloudshell-user@ip-10-130-67-187 ~]$ aws account get-contact-information
{
    "ContactInformation": {
        "AddressLine1": "THEREALSTUFF",
        "City": "Silver Spring",
        "CompanyName": "Free Code Camp",
        "CountryCode": "US",
        "FullName": "Brianna Steele",
        "PhoneNumber": "THEREASTUFF",
        "PostalCode": "THEREALSTUFF",
        "StateOrRegion": "Maryland"
    }
}

bin - binary -most basic program

linux directory standard directory structure
freeBSD /usr/bin and /usr/local/bin 
/usr/bin for already preinstalled on the system 
/usr/local/bin is stuff that YOU install
in cli ls /usr/local/bin will show directories where things you put in get 

$PATH is an environement variables
these are variables that live in the environement

command to see the file is?? 

*********ENV FILE SETUP********
simply click new file -> text file and copy this into file (your credentials found from your user that you copy to a notepad for safe keeping)
export AWS_ACCESS_KEY_ID="THEREALSTUFF"
export AWS_SECRET_ACCESS_KEY="THEREALSTUFF"
export AWS_DEFAULT_REGION="us-west-2" THIS SHOULD BE US-EAST-2 LOL

Need to save environment variables to special credentials secure area on gitpod using commands in cli:
gp env AWS_ACCESS_KEY_ID="THEREALSTUFF"
for each one
Then every time you load your gitpod these variables will be ready for us every single time
To make sure you know your env variable are set up you can go to gitpod.io dashboard then profile -> user settings and it shows the different projects env variables if you try to EDIT a variable it will show you the value of your env variable!!!!!

Had a problem where it wasn't pushing to my github. Found a gitpod community that said you have to go to user Settings and edit permissions for github bristeele99 to add "write-public-access"

