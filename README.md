# WindevMobileTools
Tools to ease Windev Mobile 25 programming

Importer la librairie .AAR dans votre projet Windows Mobile 25.

Et importer dans le code Java dans le projet WM25 par :

import com.wdlib.tools.WindevTools;

Envoi d'un SMS :

WindevTools.getInstance().SendSMS(getContexteApplication(), tel, msg);

Obtenir la mémoire libre en pourcentage :

WindevTools.getInstance().getFreeMemoryPercentage(getContexteApplication());

getTotalMemory

getTotalMemory

systemExec
