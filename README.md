# ansible-reference
Ansible snippets that I have found useful in my day to day work

**asa-config-fromjson.yml** configure object group membership using JSON data from an external file

**asa-config-loop** configure object group membership by looping over a list using with_items

**asa-config** configure object group membership with a list of lines

**findipaddrs.yml** use the ios_facts module to prepare a JSON report of all configured IP addresses on network devices. Includes file manipulation operations.

**ios_command-with-templates.yml** use ios_command iosxr_command to gather show output and then dump to a file using a jinja template and the template filter. See showcommand.j2 below.

**ios_config-example.yml** use the ios_config module to make config changes in global config as well as configuration submodes

**ios_vrf.yml** compare the ios_config and ios_vrf modules, showing ios_vrf's limitations (as of Ansible 2.4. 2.5 is supposed to add things like route targets to ios_vrf)

**l1-ios.yml** example of a provider dict

**mple-te-base.yml** build global MPLS-TE configurations on IOS-XE and IOS-XR using save_when and parents options

**multi-traceroute.yml:** run a traceroute from multiple remote linux servers to multiple destinations and send the output to a slack channel

**password-change.yml:** using ansible-vault to encrypt secrets, update passwords with ios_config and iosxr_config modules

**revert-lab.yml:** easily reset IOS-XR and IOS-XE lab routers to a clean configuration, based on a file name on a TFTP server

**save-configs-withtags.yml:** same as save-configs.yml below, but using a different tag for each task to demonstrate tag usage

**save-configs.yml:** save configurations on IOS-XR and IOS-XE routers to a TFTP server

**showcommand.j2:** Jinja temlate for use with ios_command-with-templates.yml, above.

**ssh-key-mgmt.yml:** manage ssh keys, imported into other playbooks to keep things clean - taken from
https://github.com/ipspace/NetOpsWorkshop/blob/master/tools/ssh-keys/get-keys.yml

**vars_example_1.yml:** show how to use vars stored directly in the inventory file
