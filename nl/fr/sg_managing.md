---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gestion des groupes de sécurité
{: #managing-sg}

Vous pouvez gérer les groupes de sécurité sur la page Groupes de sécurité du portail client.
{:shortdesc}

## Gestion des groupes de sécurité à partir de la page Groupes de sécurité

Pour gérer les groupes de sécurité à partir de la page Groupes de sécurité, procédez comme suit :
{:shortdesc}

1. Dans le [Portail client ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/), sélectionnez **Sécurité -> Sécurité du réseau -> Groupes de sécurité**.
2. Dans la section Groupe de sécurité, vous pouvez effectuer plusieurs tâches de gestion.
     * Afficher la liste des groupes de sécurité.
     * Créer un groupe.
     * Editer les informations sur le groupe.
     * Dupliquer un groupe.
     * Supprimer un groupe.
     
## Gestion des règles de groupe de sécurité à partir de la page Groupes de sécurité

Pour gérer les règles de groupe de sécurité à partir de la page Groupes de sécurité, procédez comme suit :
{:shortdesc}

1. Dans le [Portail client ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/), sélectionnez **Sécurité -> Sécurité du réseau -> Groupes de sécurité**.
2. Cliquez sur le nom d'un groupe de sécurité pour ouvrir la page Détails.
3. Dans la page qui s'ouvre, vous pouvez effectuer plusieurs tâches de gestion.
     * Afficher la liste des règles qui sont définies pour le groupe de sécurité.
     * Créer des règles.
     * Editer une règle.
     * Supprimer une règle.
     * Afficher les instances de serveur virtuel et les interfaces associées qui sont affectées au groupe de sécurité.
     
**Astuce :** si vous supprimez la dernière règle d'un groupe de sécurité, aucun trafic entrant ni sortant n'est autorisé par ce groupe de sécurité.
     
## Gestion des groupes de sécurité à partir de la page Détails

Pour gérer les groupes de sécurité à partir de la page Détails de l'unité, procédez comme suit :
{:shortdesc}

1. Dans le [Portail client ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/), sélectionnez **Unités -> Liste des unités**.
2. Sélectionnez le nom d'unité du serveur virtuel que vous avez commandé. La page Détails de l'unité s'ouvre.
3. Dans la page Détails de l'unité, vérifiez que vous êtes dans l'onglet **Configuration**.
4. Dans la section Groupe de sécurité, vous pouvez effectuer plusieurs tâches de gestion.
     * Afficher les groupes de sécurité et les règles.
     * Affecter les groupes de sécurité à une interface réseau d'une instance de serveur virtuel.
     * Supprimer des groupes de sécurité d'une interface réseau d'une instance de serveur virtuel.
     
     **Important** : lorsque vous affectez un groupe de sécurité existant à une interface réseau (publique ou privée) pour la première fois, vous devez redémarrer chacune des interfaces.  Toutefois, si les interfaces publique et privée ont été affectées simultanément au groupe de sécurité, un seul redémarrage est requis.  Après le redémarrage du système, les modifications sont automatiquement appliquées.
     
     Lorsque vous affectez un nouveau groupe de sécurité, celui-ci bloque l'établissement de nouvelles connexions en fonction des définitions de règles du groupe de sécurité. Toutefois, certaines connexions socket ne sont pas terminées.

     **Astuce** : si vous supprimez le dernier groupe de sécurité qui est affecté à une instance de serveur virtuel, le trafic de ce serveur n'est plus limité par les groupes de sécurité. Il n'existe plus aucun pare-feu.
     
6. Une fois les modifications terminées, cliquez sur **Sauvegarder**.
