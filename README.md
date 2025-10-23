# network_connectivity_test

ansible-playbook -i hosts test_ping_telnet.yml

**#Output Example**
TASK [Display Ping Results] *************************************************
ok: [localhost] => (item=8.8.8.8) =>
  msg: |
    PING Result for 8.8.8.8:
    2 packets transmitted, 2 received, 0% packet loss
ok: [localhost] => (item=1.1.1.1) =>
  msg: |
    PING Result for 1.1.1.1:
    2 packets transmitted, 2 received, 0% packet loss

TASK [Display Telnet Results] ***********************************************
ok: [localhost] =>
  msg: |
    TELNET Result - Destination: 8.8.8.8 Port: 80
    Status: Connected
ok: [localhost] =>
  msg: |
    TELNET Result - Destination: 8.8.8.8 Port: 22
    Status: Failed
