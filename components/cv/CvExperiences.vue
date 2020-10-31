<template>
  <div class="p-5 border-b border-grey-100">
    <h3 class="text-blue-400 font-semibold text-sm uppercase tracking-widest">
      Dernières expériences
    </h3>
    <CvExperience
      v-for="(experience, index) in experiences"
      :key="index"
      :context="experience.context"
      :client="experience.client"
      :description="experience.description"
      :from="experience.from"
      :to="experience.to"
      :tags="experience.tags"
    />
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      experiences: [
        {
          context: 'Freelancing · Full stack',
          client: 'Mobstock',
          description: `
          Reprise et refonte d'un site événementiel sous Laravel permettant l'inscription d'utilisateurs à un évènement (avec matching de disponibilités, départements, villes).
          </br>
          </br>
          Mission réalisée sur Malt.`,
          from: new Date(2020, 7),
          to: new Date(2020, 8),
          tags: [
            {
              name: 'Laravel',
            },
            {
              name: 'Vue.js',
            },
            {
              name: 'API',
            },
            {
              name: 'JavaScript',
            },
            {
              name: 'HTML5',
            },
            {
              name: 'CSS3',
            },
            {
              name: 'SASS',
            },
            {
              name: 'jQuery',
            },
          ],
        },
        {
          context: 'Freelancing · Full stack',
          client: 'Keeplove',
          description: `
          Cette mission a eu pour but dans un premier temps, d'implémenter un système d'abonnement via la solution Braintree sur un site existant, développé sous le framework Symfony 4.
          </br>
          </br>
          Dans un second temps j'ai également implémenté l'envoi de nombreux mails transactionnels via la solution SendInBlue.
          </br>
          </br>
          Et enfin, nous avons simplifié de nombreux formulaires pour les rendre plus ergonomiques pour les utilisateurs.
          </br>
          </br>
          Mission réalisée sur Malt.`,
          from: new Date(2020, 2),
          to: new Date(2020, 3),
          tags: [
            {
              name: 'Symfony',
            },
            {
              name: 'Vue.js',
            },
            {
              name: 'JavaScript',
            },
            {
              name: 'HTML5',
            },
            {
              name: 'CSS3',
            },
            {
              name: 'SASS',
            },
            {
              name: 'Bootstrap',
            },
            {
              name: 'jQuery',
            },
          ],
        },
        {
          context: 'Bug Hunter',
          client: 'YesWeHack',
          description: `
          Pentester sur la plateforme YesWeHack, je cherche et signale des vulnérabilités de sécurité sur mon temps libre à travers des rapports détaillés permettant à des entreprises de sécuriser leurs sites web.
          </br>
          </br>
          - Réalisation de test d'intrusion (Black Box, Grey Box, White Box, Scopes, Qualifying vulnerabilities / Non-qualifying vulnerabilities, etc.)
          </br>
          - Rédaction de rapports détaillés (description, exploitation, PoC, risques, recommandations, CVSS)
          </br>
          - Rédaction d'articles dans un esprit de contribution de veille informationnelle sur <a href="https://medium.com/@thibeaultchenu">https://medium.com/@thibeaultchenu</a>
          </br>
          </br>
          ➡️ une experience passionnante et addictive
          `,
          from: new Date(2020, 5),
          to: new Date(),
          tags: [
            {
              name: 'Audit de sécurité',
            },
            {
              name: 'Bug Bounty',
            },
          ],
        },
        {
          context: 'Apprenticeship - Full stack',
          client: 'Kerudys',
          description: `
          Développeur full-stack au sein d'une PME offrant ses services de consulting pour des entreprises de toute taille.
          </br>
          </br>
          - Développement full-stack : évolutions, refontes et maintenances de projets sous PHP 5 et 7 (from scratch, Laravel, Wordpress) avec connectivité SAP, LDAP, Oracle, MongoDB, MariaDB, Algolia, SendinBlue, Mailjet, réalisation de code review et peer programming, création de documentation technique, migration de Laravel 6 à 7...
          </br>
          </br>
          - Recrutement : participation et réalisation d'entretiens d'embauche
          </br>
          </br>
          - Sécurité : audit de sécurité des projets existants, corrections, DevOps -> DevSecOps
          </br>
          </br>
          - Utilisation de tâches JIRA (Scrum et Kanban) et de Slack
          </br>
          </br>
          ➡️ une expérience enrichissante de part ses défis techniques et les responsabilités accordées
          `,
          from: new Date(2019, 8),
          to: new Date(),
          tags: [
            {
              name: 'Laravel',
            },
            {
              name: 'Vue.js',
            },
            {
              name: 'JavaScript',
            },
            {
              name: 'HTML5',
            },
            {
              name: 'CSS3',
            },
            {
              name: 'SASS',
            },
            {
              name: 'Bootstrap',
            },
            {
              name: 'TailwindCSS',
            },
            {
              name: 'jQuery',
            },
            {
              name: 'API',
            },
            {
              name: 'Redis',
            },
            {
              name: 'MongoDB',
            },
            {
              name: 'Wordpress',
            },
            {
              name: 'Algolia',
            },
            {
              name: 'Transactional Emails',
            },
            {
              name: 'Marketing campaigns',
            },
            {
              name: 'Mailjet',
            },
            {
              name: 'Sendinblue',
            },
            {
              name: 'Job interviews',
            },
            {
              name: 'Refactoring',
            },
            {
              name: 'Migration',
            },
          ],
        },
        /*
        {
          context: 'Agency - Full stack',
          client: "Ministère de l'Intérieur",
          description: `
          Cette mission pour le ministère de l'intérieur a eu pour but de développer la nouvelle version du portail candidat.
          </br>
          </br>
          Le portail candidat est un webcomponent VueJS couplé à une API développée sous le framework PHP Symfony permettant à des millions de français de télécharger leurs résultats aux permis de conduire.
          </br>
          </br>
          Ce portail candidat est disponible sur le site de la sécurité routière.
          </br>
          </br>
          Mission réalisée par le biais de l'agence Maecia.
          `,
          from: new Date(2018, 7),
          to: new Date(2018, 11),
        },
        {
          context: 'Freelancing - Full stack',
          client: 'Galaxie Media',
          description: `
          Cette mission de 1 mois a consisté à migrer le forum Tom'sGuide et Tom'sHardware France développés tout deux sous le framework PHP Symfony vers le CMS xenForo.
          </br>
          </br>
          J'ai été amené à créer un processus de migration de données adapté à l'architecture de la base de données relationnelle MySQL des deux forums. 
          </br>
          </br>
          Outre les données à migrer, j'ai également été amené à migrer différentes fonctionnalités sous la forme de modules.
          `,
          from: new Date(2018, 9),
          to: new Date(2018, 10),
        },
        {
          context: 'Agency - Full stack',
          client: 'Maecia',
          description: `
          Développeur back-end au sein d'une ESN offrant ses services pour des clients de toute taille (AFP, Banque BCP, Groupe Arching, Engie, Ministère de l’Intérieur…)
          </br>
          </br>
          - Développement backend : évolutions et maintenance de projets sous divers technologies comme Drupal 7 & 8, Laravel ou encore Lumen.
          </br>
          - Sécurité : audit de sécurité de la solution d'intranet Inside, mise en place de corrections et recommandations
          </br>
          - Utilisation de tâches Trello, JIRA et Bitbucket et du service de communication Slack destiné à la gestion des projets
          </br>
          </br>
          ➡️ une expérience enrichissante et unique.
          `,
          from: new Date(2017, 8),
          to: new Date(2019, 8),
        },
        {
          context: 'Volunteer - Full stack',
          client: 'Induste',
          description: `
          Développeur d'une structure à fort traffic (site web classé 1'500ième en France au classement Alexa (20ième dans sa catégorie) , 900'000 membres inscrits et plus de 80'000 visiteurs par jour).
          </br>
          - Développement "full-stack" : backend PHP framework xenForo basé sur Zend2, bases de données relationnelles MySQL, frontend HTML / CSS / JS.
          </br>
          - Utilisation poussée de tâches Trello & du service de communication Slack destinés à la gestion des projets internes à la structure : supports opérationnels aux équipes.
          </br>
          </br>
          => une expérience très complète en informatique, développement.
          `,
          from: new Date(2017, 8),
          to: new Date(2019, 8),
        },
        */
      ],
    }
  },
}
</script>
