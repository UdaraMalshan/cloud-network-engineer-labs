I have practiced in this lab about,
     
         1)Configure Cisco router as DHCP server
         2)Router Configure as DHCP client
         3)Configure DHCP relay agent
         4)Also troubleshooting with my own lab

Commands I have been used,
       
      01)Define reserve ip address range,
   
            ip dhcp excluded-address -------   --------
        
      02)Define DHCP pools,
  
            ip dhcp pool POOL1
            network 192.168.1.0 255.255.255.0
            dns-server 8.8.8.8
            default-router 192.168.1.1
            domain-name malshanlab.com

      03)Configure DHCP client
    
            ip address dhcp
            no shutdown

      04)Configure DHCP Really agent
            
            ip helper-address -dhcp server address-


      05)I also use static routing commands for route the both routers.
           
            Ip route 192.168.2.0 255.255.255.0 g0/0