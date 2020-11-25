# WindevMobileTools
# Librairie facilitant le développement Android sous Windev Mobile 25 #

Importer la librairie .AAR dans votre projet Windows Mobile 25.

Et importer dans le code Java dans le projet WM25 par :

import com.reuniware.windevmobiletools.WindevMobileTools;

# Supprimer mode Device Owner #

WindevMobileTools.getInstance().RemoveDeviceOwner(getContexteApplication());

# Démarrer Chrome #

WindevMobileTools.getInstance().StartChrome(getActiviteEnCours(), "https://ntic974.blogspot.com");

# Envoi d'un SMS (sans la permission SEND_SMS) #

WindevMobileTools.getInstance().SendSMS(getActiviteEnCours(), "+330101010101", "Message de test");

# Obtenir la mémoire libre en pourcentage #

double mem = WindevMobileTools.getInstance().GetFreeMemoryPercentage(getContexteApplication());

# Obtenir la mémoire totale #

double mem = WindevMobileTools.getInstance().GetTotalMemory(getContexteApplication())

# Obtenir la mémoire disponible #

double mem = WindevMobileTools.getInstance().GetAvailableMemory(getContexteApplication())

# Exécuter une commande shell #

String result = WindevMobileTools.getInstance().SystemExec("ls")

# AndroidMgrClient.apk #

Cet outil est en cours de développement et démarre un serveur de socket sur le port 8000 sur l'Android. On peut alors se connecter sur l'Android depuis en PC en ligne de commande en entrant "telnet 192.168.1.200 8000", en remplaçant "192.168.1.200" par l'adresse IP de votre téléphone Android.

On peut alors lancer les commandes suivantes (la liste va évoluer) :

repexe : Retourne le répertoire d'exécution de l'application

repencours : Retourne le répertoire en cours de l'application

fichiers : Liste les fichiers dans le répertoire en cours

repertoires : Liste les répertoires dans le répertoire en cours

nbsms : Retourne le nombre de SMS en mémoire

getsms : Obtient le premier SMS

getnextsms : Obtient le SMS suivant

getallsms : Obtient tous les SMS

