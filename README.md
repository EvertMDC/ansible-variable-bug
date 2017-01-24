# ansible-variable-bug

This is either a bug in Ansible or I don’t see my error.
It’s a playbook that launches a role 2 times, first with testvalue = true, testvalue2=false. Afterwards with testvalue = false, testvalue2 = true.
When using or printing out the variables, it prints true - false, true - false twice instead of using the adapted variables.

The values are changed if the type changes. For example by first using a bool 
"testvalue = true"
and afterwards a string
testvalue = "false"
