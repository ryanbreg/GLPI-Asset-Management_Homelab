GLPI asset inventory with Netalertx network management
  
  I built a homelab management software duo to keep track of all computers and equipment along with their network connection statuses and device info(IP addresses, Mac addresses...)

I started off by configuring a Debian GLPI inventory server, and subsequently installed GLPI agents on each of my homelab computers and virtual machines. For any of my agentless devices(printer, managed switch) I used network discovery via SNMP running through the Debian agent to a specified IP address. All other devices and monitors were manually created in the inventory. 

Troubleshooting Areas

While configuring my Epson printer to accept network discovery, the agent was installed and available, but not listed as an available choice for network discovery. Through some trial and error I found that the plugin for network discovery was disabled.

My future goals for this management software are to keep inventory of any hardware or components that are added and updated as I continue to build my homelab, and to have a reliable, accurate database to reference when troubleshooting any problems in my network.

<img width="991" height="949" alt="Screenshot 2026-11-09 192600" src="https://github.com/user-attachments/assets/9e711065-8dc2-4c7a-ba58-02e1fd0ea9af" />

