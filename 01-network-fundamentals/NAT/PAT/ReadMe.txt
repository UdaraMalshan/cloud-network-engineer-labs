I have practiced in this lab about,
     
         1)Configure PAT
         2)Source NAT

Commands I have been used,
       
      01)Define inside & outside interfaces for NAT,
   
            int g0/0
            ip nat inside/outside
        
      02)configure ACL to limit the access,
  
            access-list 1 permit 172.16.0.0. 0.0.0.255

      03)Map the ACL to router's interface as PAT

            ip nat inside source list 1 interface g0/0 overload

      04)show current NAT configs,
    
            show ip nat translations


      05)I also use static routing commands for route the both routers.
           
            Ip route 192.168.2.0 255.255.255.0 g0/0