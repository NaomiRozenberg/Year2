```
routing_table = {}
next_ip = "192.168.0.1"

def is_valid_mac(mac):
    parts = Split mac by ':'
    
    If length of parts != 6:
        return False
    
    For each part in parts:
        If length of part != 2:
            return False
    return True

def manage_routing_table(mac_add):
    If mac_add in routing_table:
        Print "MAC already exists. IP Address: " + routing_table[mac_add]
    Else:
        routing_table[mac_add] = next_ip
        Print "New entry added. IP Address: " + next_ip
        next_ip = get_next_ip(next_ip)

    Print "Routing Table:"
    For mac in routing_table:
        Print mac + " -> " + routing_table[mac]

While True:
    mac_add = Input "Enter a MAC address (or type 'exit' to stop): "
    If mac_add == "exit":
        Break
    manage_routing_table(mac_add)

```
