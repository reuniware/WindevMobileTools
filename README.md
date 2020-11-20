# WindevMobileTools
# Librairie facilitant le développement Android sous Windev Mobile 25 #

Importer la librairie .AAR dans votre projet Windows Mobile 25.

Et importer dans le code Java dans le projet WM25 par :

import com.reuniware.windevmobiletools.WindevMobileTools;

# Envoi d'un SMS #

WindevMobileTools.getInstance().SendSMS(getContexteApplication(), "+330101010101", "Message de test");

# Obtenir la mémoire libre en pourcentage #

double mem = WindevMobileTools.getInstance().GetFreeMemoryPercentage(getContexteApplication());

# Obtenir la mémoire totale #

double mem = WindevMobileTools.getInstance().GetTotalMemory(getContexteApplication())

# Obtenir la mémoire disponible #

double mem = WindevMobileTools.getInstance().GetAvailableMemory(getContexteApplication())

# Exécuter une commande shell #

String result = WindevMobileTools.getInstance().SystemExec("ls")

# AndroidMgrClient.apk #

Cet outil est en cours de développement et démarre un serveur de socket sur le port 8000 sur l'Android. On peut alors de connecter sur l'Android depuis en PC en ligne de commande en entrant "telnet 192.168.1.200 8000", en remplaçant "192.168.1.200" par l'adresse IP de votre téléphone Android.
