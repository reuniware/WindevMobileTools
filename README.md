# WindevMobileTools
#Librairie facilitant le développement Android sous Windev Mobile 25#

Importer la librairie .AAR dans votre projet Windows Mobile 25.

Et importer dans le code Java dans le projet WM25 par :

import com.reuniware.windevmobiletools.WindevTools;

Envoi d'un SMS :

WindevTools.getInstance().SendSMS(getContexteApplication(), "+330101010101", "Message de test");

Obtenir la mémoire libre en pourcentage :

WindevTools.getInstance().GetFreeMemoryPercentage(getContexteApplication());

Obtenir la mémoire totale :

WindevTools.getInstance().GetTotalMemory(getContexteApplication())

Obtenir la mémoire disponible :

WindevTools.getInstance().GetAvailableMemory(getContexteApplication())

Exécuter une commande shell :

WindevTools.getInstance().SystemExec("ls")
