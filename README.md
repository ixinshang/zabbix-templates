# Advanced zabbix-template for monitoring network devices
Template switch_universal: UPDATED, version 6.2
- Based on SNMPv2 Network template
- SNMP Community now defined by macros
- 2 LLDs: standard\extended. UPPERCASE interface description used to extended checks. Use regexp:^[A-Z \d\W]+$	[Result is TRUE] 
- Removed SNMP Traps (moved to another template)
- Removed all calculated items
---
Template config_manager:
- Send SNMPSET request to device, monitoring result

---
Template ICMP ping Base
- Base template, with removed 2 items. Triggers patched.

---
Template ICMP ping Advanced
- Based on smokeping template. Added 2 triggers, 1 linked template.
