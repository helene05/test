+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
1- Ce Projet consiste a classifier les malawares de facon static
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Nous utiliserons des outils pour arriver a notre fin.
Vous trouverez des malwares dans le dosiier malwares.
vous trouverez egalement certains fichiers .png qui reprentent les images des appels de 
fonction des malwares.

***************************************************************************************

++++++++++++++++++++++++++++++ AVERTISSEMENT ++++++++++++++++++++++++++++++++++++++++++

LE DOSSIER MALWARES CONTIENT DES MALWARES CAPABLES DE S'EXECUTER AVEC LES DIFFERENTS TYPES DE PROCESSEURS.

LES ETAPES DE REALISATIONS DU PROJET :

///////////////    ETAPE1 /////////////////////////////////

1- CE PROJET PERMET DE FAIRE UNE CLASSIFICATION STATIQUE DES MALWARES SELON : 

    A-SIGNATURE , B-FORMAT , C-TYPE DE FICHIER , D-DESSEMBLAGE , E-DECOMPILATION

2-NOUS AVONS UTILISÉS CERTAINS OUTILS POUR REALISER CES TACHES.

         A-REDIS POUR GERER AUTOMATIQUEMENT LA STRUCTURE DES MALWARES ET LEUR SAUVEGARDE DANS UNE BDD
         B-GEPHI POUR VISUALISER LES APPELS DE FONCTION D'UN MALWARES COMME UN GRAPHE
         C-LE SITE virustotal.com NOUS A PERMIS DE RETROUVER LES SIGNATURES DES MALWARES.
         D-BEAUCOUP DE COMMANDES LINUX POUR COMPARER , VISUALISER , TRAITER ET CREATION DES FICHIER .
         
/////////////    ETAPE 2 //////////////////////////
   
3- LES LIGNES DE COMMANDES :

      a- creation de deux fichiers de malwares :
           objdump -d d603d7933b3fe94dbadb21e19f574459738f53b6080561f2c4a71a1b0116c9ff > malware1
           objdump -d fff7ba61cd15eb76a8e2098c71182925d2bcb1b8e0d9aa296d5f61521bfa184d > malware2
      b- comparer deux malwares :
           diff malware1 malware2 
      c- trouver la SIGNATURE des malwares :
           virustotal.com ( les signatures non trouvées sont ajoutées à AIL FRAMEWORK
      d- DECOMPILATION des malwares :
      
