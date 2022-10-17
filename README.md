# HCX-MultiSite-Deploy

# HCX-MultiSite-Deploy

This is a PowerShell 5.1 Script designed to Install, Activate, Configure HCX in two Sites.

Written By Heath Johnson & Ben Sier

Functions for HCX API Calls By William Lam


######-- Pre-reqs --############

Script Tested and Runs in PowerShell 5.1

PowerShell 7.x does not work for this version of the Script.

PowerCli 12.7

Two vSphere Sites that you want to connect with HCX
Note: This has been Developed and tested with two VCF 4.4 sites using the VLC

DNS is a critical component for this script to be successful
DNS must work for resolving the DNS names of all vSphere and NSX components in both Sites, as well as DNS connectivity to the intenet for HCX Cloud Activation
Don't forget to put in DNS entries for the HCX manager deployed by this script.

Windows Jumphost with Network Access to Both Sites and can DNS resolve all vSphere and NSX in both sites

Download the HCX Cloud OVA appliance

HCX License Keys


###############################

To use the script, download the Ps1 Script and the associated .ini input file

Completely fill out all fields in the ini file to match your environments. Any minor typos will cause the script to error.

Launch the script from your jumphost.
a Windows File Explorer window will pop open, Select the ini input file and the script will begin.

Individual sections of the script can be enabled and disabled so that if you get part way through and have an error due to a typo, you can pick up where your left off.

