 A.Symétrique  

Adresse de réseau de base est  172.16.1.0/24 ==> donc 32-24 = 8 donc  2^8 =  256 adresses possibles

On divise en 4 le nombre de sous-réseaux égaux  donc 64 pour chaque Pole 


| Pole                | Adresse Réseau | CIDR       | Adresse Broadcast   |
|---------------------|-----------------|------------|---------------------|
| Informatique        | 172.16.1.0      | 172.16.1.0/26  | 172.16.1.63      |
| Développement       | 172.16.1.64     | 172.16.1.64/26 | 172.16.1.127     |
| Administratif       | 172.16.1.128    | 172.16.1.128/26 | 172.16.1.191     |
| Technicien          | 172.16.1.192    | 172.16.1.192/26 | 172.16.1.255     |

B.Asymétrique

   | Pole                | Adresse Réseau  | CIDR           | Adresse Broadcast   |
|---------------------|-----------------|----------------|---------------------|
| Informatique        | 172.16.1.0      | 172.16.1.0/26  | 172.16.1.63        |
| Développement       | 172.16.1.64     | 172.16.1.64/28 | 172.16.1.79        |
| Administratif       | 172.16.1.80     | 172.16.1.80/27 | 172.16.1.111       |
| Technicien          | 172.16.1.112    | 172.16.1.112/28 | 172.16.1.127       |


Explication :

Informatique  c'est 50 équipements  2^6= 64 adresses   CIDR : /26

  Développement : 12 équipements     2^4=16 adresses     CIDR  : /28
  
 Administratif : 20 équipements    2^5= 32 adresses     CIDR : /27

 Technicien : 15 équipements    2^4= 16 adresses        CIDR :/28
