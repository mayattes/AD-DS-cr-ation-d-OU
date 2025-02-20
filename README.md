# AD-DS création d'Unité d'Organisation

### Étape 1 : Créer une Unité d'Organisation (OU) - `Wilders_students`

**Ouvrir "Active Directory Users and Computers"**
   - Ouvrir le menu Démarrer et rechercher **Active Directory Users and Computers**.
   - Lancer l'application.

**Naviguer vers le domaine Wilders.lan**
   - Dans le volet gauche, repérez **wilders.lan**.
   - Clic droit sur **wilders.lan** et sélectionner **New** > **Organizational Unit**.

**Nommer l'OU**
   - Dans la fenêtre **New Organizational Unit**, entrez **Wilders_students** comme nom.
   - Cliquez sur **OK**.

---

### Étape 2 : Créer un Groupe d'Utilisateurs - `Students`

**Naviguer vers l'OU Wilders_students**
   - Dans le volet gauche, localisez l'OU **Wilders_students** sous **wilders.lan**.

**Créer le groupe**
   - Clic droit sur **Wilders_students**, puis sélectionnez **New** > **Group**.
   
**Configurer le groupe**
   - Dans la fenêtre **New Object - Group**, entrez **Students** comme nom de groupe.
   - Sélectionnez **Global** comme type de groupe.
   - Pour le **Scope**, choisissez **Security**.
   - Cliquez sur **OK** pour créer le groupe.

---

### Étape 3 : Créer un Utilisateur au sein du groupe `Students`

**Créer un nouvel utilisateur**
   - Clic droit sur **Wilders_students**, puis sélectionnez **New** > **User**.

**Configurer les informations de l'utilisateur**
   - Dans la fenêtre **New Object - User**, renseignez les informations de l'utilisateur :
     - **First Name**: Exemple : `John`
     - **Last Name**: Exemple : `Doe`
     - **User logon name**: Exemple : `jdoe`
   
   - Cliquez sur **Next**.

**Définir le mot de passe**
   - Définissez un mot de passe pour l'utilisateur.
   - Cochez **User must change password at next logon** si vous souhaitez forcer l'utilisateur à changer son mot de passe après sa première connexion.
   - Cliquez sur **Next** puis **Finish** pour terminer la création de l'utilisateur.

L'utilisateur **John Doe (jdoe)** est désormais créé dans l'OU **Wilders_students**.

**Ajouter l'utilisateur au groupe Students**
   - Clic droit sur l'utilisateur **John Doe** (jdoe), puis sélectionnez **Add to a group**.
   - Dans la fenêtre **Enter the object name to select**, tapez **Students** et cliquez sur **Check Names**.
   - Cliquez sur **OK** pour ajouter l'utilisateur au groupe **Students**.

---


