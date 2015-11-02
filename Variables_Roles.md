Variables - variables can come from a variety of locations.

- Playbooks
- Inventory (group vars, host vars)
- Command lines (defined when the command line is run and the variable is also referenced in other playbook)
- Discovered Variables (facts) - comes from running a module that is designed to discover information about the instance that it is being run against.
The output is returned in json.


Example of Discovery Command

ansible -m setup -u vagrant
