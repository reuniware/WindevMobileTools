# WindevMobileTools
# Librairie facilitant le développement Android sous Windev Mobile 25 #

Importer la librairie .AAR dans votre projet Windows Mobile 25.

Et importer dans le code Java dans le projet WM25 par :

import com.reuniware.windevmobiletools.WindevMobileTools;

# Envoi d'un SMS #

WindevMobileTools.getInstance().SendSMS(getContexteApplication(), "+330101010101", "Message de test");

# Obtenir la mémoire libre en pourcentage #

WindevMobileTools.getInstance().GetFreeMemoryPercentage(getContexteApplication());

# Obtenir la mémoire totale #

WindevMobileTools.getInstance().GetTotalMemory(getContexteApplication())

# Obtenir la mémoire disponible #

WindevMobileTools.getInstance().GetAvailableMemory(getContexteApplication())

# Exécuter une commande shell #

WindevMobileTools.getInstance().SystemExec("ls")
