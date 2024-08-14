<template>
  <main
    id="content"
    class="site-main post-77 page type-page status-publish hentry max-w-[1313px] mx-auto pb-10 px-4"
  >
    <div class="page-header pb-4">
      <h1 class="text-4xl">
        <font style="vertical-align: inherit"
          ><font style="vertical-align: inherit">{{ $t("legal") }}</font></font
        >
      </h1>
    </div>

    <div class="page-content space-y-4 text-2xl" v-if="locale === 'en'">
      <div class="w-full h-px bg-black"></div>

      <p>
        <strong
          ><font style="vertical-align: inherit"
            ><font style="vertical-align: inherit" class=""
              >Name of company/organization:</font
            ></font
          ></strong
        ><font style="vertical-align: inherit"
          ><font style="vertical-align: inherit" class="">
            LIMA PROTECTION</font
          ></font
        >
      </p>

      <p>
        <strong
          ><font style="vertical-align: inherit"
            ><font style="vertical-align: inherit">Email address:</font></font
          ></strong
        ><font style="vertical-align: inherit"
          ><font style="vertical-align: inherit">
            contact@limaprotection.com</font
          ></font
        >
      </p>

      <p>
        <strong
          ><font style="vertical-align: inherit"
            ><font style="vertical-align: inherit">Site host:</font></font
          ></strong
        ><font style="vertical-align: inherit"
          ><font style="vertical-align: inherit"> GoDaddy</font></font
        >
      </p>

      <ul class="wp-block-list">
        <li>
          <strong
            ><font style="vertical-align: inherit"
              ><font style="vertical-align: inherit">Host address:</font></font
            ></strong
          ><font style="vertical-align: inherit"
            ><font style="vertical-align: inherit">
              United States Tempe 2155 E. GoDaddy Way HQ</font
            ></font
          >
        </li>

        <li>
          <strong
            ><font style="vertical-align: inherit"
              ><font style="vertical-align: inherit"
                >Host telephone number:</font
              ></font
            ></strong
          ><font style="vertical-align: inherit"
            ><font style="vertical-align: inherit"> 1-480-366-3546</font></font
          >
        </li>
      </ul>

      <h2 class="wp-block-heading">
        <font style="vertical-align: inherit"
          ><font style="vertical-align: inherit"
            >Intellectual Property</font
          ></font
        >
      </h2>

      <p>
        <font style="vertical-align: inherit"
          ><font style="vertical-align: inherit"
            >The content of this site, including texts, images, graphics and
            logo, is the property of Lima Protection and is protected by
            intellectual property laws. Any reproduction, modification,
            publication or adaptation of all or part of the elements of the
            site, whatever the means or process used, is prohibited without
            prior written authorization from Lima Protection.</font
          ></font
        >
      </p>

      <h2 class="wp-block-heading">
        <font style="vertical-align: inherit"
          ><font style="vertical-align: inherit"
            >Limitation of Liability</font
          ></font
        >
      </h2>

      <p>
        <font style="vertical-align: inherit"
          ><font style="vertical-align: inherit"
            >Lima Protection cannot be held responsible for direct or indirect
            damage caused to the user's equipment when accessing the
            limaprotection.com site, and resulting either from the use of
            equipment not meeting the specifications indicated, or from the
            appearance of a bug or incompatibility.</font
          ></font
        >
      </p>

      <p>
        <font style="vertical-align: inherit"
          ><font style="vertical-align: inherit"
            >[Company Name] cannot also be held responsible for indirect damage
            (such as loss of market or loss of opportunity) resulting from the
            use of the [Site Name] site.</font
          ></font
        >
      </p>

      <h2 class="wp-block-heading">
        <font style="vertical-align: inherit"
          ><font style="vertical-align: inherit"
            >Applicable Law and Attribution of Jurisdiction</font
          ></font
        >
      </h2>

      <p>
        <font style="vertical-align: inherit"
          ><font style="vertical-align: inherit"
            >Any dispute relating to the use of the limaprotection.com site is
            subject to French law. In the event of a dispute, the French courts
            will have jurisdiction.</font
          ></font
        >
      </p>

      <h2 class="wp-block-heading">
        <font style="vertical-align: inherit"
          ><font style="vertical-align: inherit"
            >Modification of Legal Notices</font
          ></font
        >
      </h2>

      <p>
        <font style="vertical-align: inherit"
          ><font style="vertical-align: inherit"
            >Lima Protection reserves the right to modify these legal notices at
            any time. The user is invited to consult them regularly.</font
          ></font
        >
      </p>
    </div>

    <div class="page-content space-y-4 text-2xl" v-else>
      <div class="w-full h-px bg-black"></div>

      <p><strong>Nom de l’entreprise/organisation :</strong> LIMA PROTECTION</p>

      <p><strong>Adresse e-mail :</strong> contact@limaprotection.com</p>

      <p><strong>Hébergeur du site :</strong> GoDaddy</p>

      <ul class="wp-block-list">
        <li>
          <strong>Adresse de l’hébergeur :</strong> United States Tempe 2155 E.
          GoDaddy Way HQ
        </li>

        <li>
          <strong>Numéro de téléphone de l’hébergeur :</strong> 1-480-366-3546
        </li>
      </ul>

      <h2 class="wp-block-heading">Propriété Intellectuelle</h2>

      <p>
        Le contenu de ce site, incluant les textes, images, graphismes et logo,
        est la propriété de Lima Protection et est protégé par les lois sur la
        propriété intellectuelle. Toute reproduction, modification, publication
        ou adaptation de tout ou partie des éléments du site, quel que soit le
        moyen ou le procédé utilisé, est interdite, sauf autorisation écrite
        préalable de Lima Protection.
      </p>

      <h2 class="wp-block-heading">Limitation de Responsabilité</h2>

      <p>
        Lima Protection ne peut être tenu responsable des dommages directs ou
        indirects causés au matériel de l’utilisateur lors de l’accès au site
        limaprotection.com, et résultant soit de l’utilisation d’un matériel ne
        répondant pas aux spécifications indiquées, soit de l’apparition d’un
        bug ou d’une incompatibilité.
      </p>

      <p>
        [Nom de l’Entreprise] ne pourra également être tenu responsable des
        dommages indirects (tels qu’une perte de marché ou perte d’une chance)
        consécutifs à l’utilisation du site [Nom du Site].
      </p>

      <h2 class="wp-block-heading">
        Droit Applicable et Attribution de Juridiction
      </h2>

      <p>
        Tout litige en relation avec l’utilisation du site limaprotection.com
        est soumis au droit français. En cas de litige, les tribunaux français
        seront compétents.
      </p>

      <h2 class="wp-block-heading">Modification des Mentions Légales</h2>

      <p>
        Lima Protection se réserve le droit de modifier ces mentions légales à
        tout moment. L’utilisateur est invité à les consulter régulièrement.
      </p>
    </div>
  </main>
</template>

<script setup>
import { useI18n } from "vue-i18n";
const { locale } = useI18n();

definePageMeta({
  layout: "white",
});
</script>

<style scoped>
h2 {
  @apply text-4xl py-2;
}
</style>
