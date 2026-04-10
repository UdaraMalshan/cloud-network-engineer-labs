I have practiced in this lab about,
     
         1)Configure static NAT(one to one mapping)
         2)Source NAT

Commands I have been used,
       
      01)Define inside & outside interfaces for NAT,
   
            int g0/0
            ip nat inside/outside
        
      02)Map one local ip to one global ip,
  
            ip nat inside source static -local ip add- -mapped global ip add-

      03)show current NAT configs,
    
            show ip nat translations


      04)I also use static routing commands for route the both routers.
           
            Ip route 192.168.2.0 255.255.255.0 g0/0