# WindevMobileTools
Tools to ease Windev Mobile 25 programming

Importer la librairie .AAR dans votre projet Windows Mobile 25.

Pour l'instant une seule fonction est disponible, et permet d'envoyer un SMS (sans nécessité d'avoir la permission android.permission.SEND_SMS.
Pour appeler cette fonction, il faut déclarer le code suivant dans Window Mobile 25 (en procédure globale) :

import com.wdlib.tools.WindevTools;

public static void EnvoyerSMS(String tel, String msg)

{

	WindevTools.getInstance().SendSMS(getContexteApplication(), tel, msg);

}

