## Prérequis & Éléments requis
* Identifiants du compte utilisateur local (mot de passe de session).
* Identifiants du compte Apple (Identifiant Apple / iCloud) associé, le cas échéant.
* Facture d'achat d'origine au nom de l'entreprise (en cas de blocage Activation Lock).

---

## Méthode 1 : Réinitialisation depuis la session macOS (Méthode Recommandée)

Si vous possédez le mot de passe de la session administrative locale :

1. Ouvrir les **Réglages Système**.
2. Aller dans **Général** > **Transférer ou réinitialiser**.
3. Cliquer sur **Effacer contenu et réglages...**
4. Saisir le mot de passe administrateur local.
5. Si un compte Apple est associé, le mot de passe de l'identifiant Apple sera demandé pour désactiver *Localiser* et l'*Activation Lock*.
6. Valider pour lancer l'effacement sécurisé et le retour à l'écran de bienvenue (Setup Assistant).

---

## Méthode 2 : Réinitialisation via le Mode Récupération (Recovery)

Si la session ne s'ouvre pas mais que vous possédez le mot de passe local et/ou le compte Apple :

### Étape 1 : Accéder au Mode Récupération
1. Éteindre complètement le Mac.
2. Maintenir le **bouton d'alimentation (Touch ID)** enfoncé jusqu'à ce que le message *"Chargement des options de démarrage..."* apparaisse.
3. Sélectionner **Options**, puis cliquer sur **Continuer**.

### Étape 2 : Authentification & Effacement
* **Si le Mac demande le mot de passe local :** Sélectionnez un utilisateur administrateur et saisissez son mot de passe.
* **Si le Mac est lié à un compte Apple :** Saisissez les identifiants Apple pour déverrouiller l'accès aux options.
* **Effacement complet :**
  1. Une fois dans le menu principal de la récupération, cliquez sur **Assistant de récupération** dans la barre des menus en haut de l'écran.
  2. Sélectionnez **Effacer le Mac...**
  3. Confirmez l'effacement. Le Mac redémarrera et se réinitialisera.
  4. Au redémarrage, connectez le Mac au Wi-Fi pour activer l'appareil, puis réinstallez macOS si demandé.

---

## Méthode 3 : Gestion du blocage "Activation Lock" (Sans accès aux identifiants)

Si vous ne possédez ni le mot de passe local ni l'accès au compte Apple associé, l'appareil est bloqué par l'**Activation Lock**.

### Option A : Retrait à distance via iCloud
Si l'ancien utilisateur/collaborateur est joignable :
1. Demandez-lui de se connecter sur [icloud.com/find](https://www.icloud.com/find).
2. Sélectionner le Mac dans la liste des appareils.
3. Cliquer sur **Effacer le Mac**, puis sur **Supprimer du compte**.
4. Une fois supprimé du compte, redémarrer le Mac et le connecter au Wi-Fi pour lever le verrouillage.

### Option B : Demande d'assistance d'activation auprès d'Apple
Si l'utilisateur est injoignable et que le Mac n'est pas géré par un MDM :
1. Se munir de la **facture d'achat originale** (doit comporter le numéro de série du Mac et le nom de l'entreprise/acheteur).
2. Soumettre une demande officielle sur le portail dédié : [al-support.apple.com](https://al-support.apple.com/#/).
3. Renseigner les coordonnées de l'entreprise et joindre la preuve d'achat.
4. *Délai de traitement :* Généralement sous 3 à 5 jours ouvrés. Une fois validé par Apple, connectez le Mac à Internet pour débloquer l'appareil.

> ⚠️ **Attention :** Les demandes soumises par un prestataire externe au nom d'un tiers sans mandat clair ou avec une facture au nom d'une autre entité sont systématiquement refusées par Apple.

---

## Absence de preuve d'achat et d'identifiants
Si l'Activation Lock est actif et qu'aucune preuve d'achat originale n'est disponible, il n'existe **aucun moyen technique ou logiciel** de contourner la protection sur les puces Apple Silicon. Le matériel est inexploitable (utilisation restreinte à la récupération de pièces détachées non chiffrées).

---

## Bonnes Pratiques d'Entreprise
* **Supervision via MDM (ABM / Intune) :** Enrôler systématiquement les équipements dans *Apple Business Manager (ABM)* et Microsoft Intune. Cela permet de contourner l'Activation Lock grâce aux clés de déverrouillage MDM (*Bypass Code*) sans dépendre du compte personnel d'un employé.
* **Politique de compte :** Restreindre la connexion des comptes iCloud personnels ou désactiver la fonction *Localiser mon Mac* via des profils de configuration Intune/MDM.
