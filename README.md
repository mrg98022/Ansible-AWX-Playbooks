---
  - name: show inter playbook
    hosts: all
    gather_facts: no
    connection: network_cli
    tasks:
      - name: run sh ip int br
        ios_command:
          commands: show ip int br
