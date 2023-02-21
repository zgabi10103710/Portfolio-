<template>
  <div class="container">


      <BinaryTextSVG />
      <h1 class="about-content__headline">Certification  </h1>

    <main id="main-content">
      <article class="about-content">
      <h1 class="about-content__headline"> Réussi  </h1>
        <p>👋 Voici la certification Try hack me passé le 26 Decembre 2022</p>
        <img src="https://tryhackme-certificates.s3-eu-west-1.amazonaws.com/THM-CMTZIEIUK9.png" />



      <h1 class="about-content__headline">En cours</h1>
      <p> La certification Complete Beginner sur try hack me et entrain d'etre passée  ( 50 %  ) </p>
      <img src="https://assets.tryhackme.com/img/paths/completebeginner-square.svg" />


      <h1 class="about-content__headline">Objetif</h1>
      <p>
      <ul>
        <li>Try hack me top 1% </li>
        <li>Hack the box : Penetration Testing Certification
          <img src="https://academy.hackthebox.com/storage/exam_splash_banners/6qCRpSH5zRrzFMH7zdLB8cYNEYDGQwIeXER9OjER.png" />
        </li>
        <li>Hack the box : Bug Bounty Hunting Certification
          <img src="https://academy.hackthebox.com/storage/exam_splash_banners/jIQOAaoXKp36Rd30F0cNgymk9UbBLmJdlWXBc8wZ.png" />
        </li>
        <li>OSAWP</li>
        <img src="        https://www.offensive-security.com/wp-content/themes/OffSecChildTheme/assets/images/hero-frame.svg" />



      </ul>
      </p>






      </article>
    </main>
  </div>
</template>

<script setup>
import { useRoute } from 'vue-router'
import config from '../config/siteconfig.json'

const title = 'About me • Gabriel Briziou '
const { description } = config
const route = useRoute()

useHead({
  title,
  meta: [
    {
      name: 'description',
      content: description,
    },
    { property: 'og:type', content: 'website' },
    { property: 'og:title', content: title },
    { property: 'og:description', content: description },
    { property: 'og:url', content: `${config.siteUrl}${route.path}` },
    {
      property: 'twitter:title',
      content: title,
    },
    {
      property: 'twitter:description',
      content: description,
    },
  ],
})
</script>

<route lang="yaml">
meta:
  layout: default
</route>

<style lang="css" scoped>
:global(#app) {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.container {
  flex-flow: row wrap;
  padding: 3rem 0;
}

main {
  padding: 1.2rem 2.4rem;
}

.about-content {
  .about-content__headline {
    font-size: var(--text-2xl);
  }

  p {
    font-size: var(--text-lg);
    opacity: 0.8;
    max-width: 71ch;
  }
}

.binary-text-svg {
  font-family: var(--font-mono);
  font-size: var(--text-xl);
  position: absolute;
  left: 282px;
  top: 387px;
  opacity: 0.3;

  & :deep(tspan) {
    --text-delay: 500ms;

    opacity: 0;
    animation: pulse-spread 3s var(--text-delay) ease-out infinite alternate;

    &:nth-child(1) {
      --text-delay: 500ms;
    }

    &:nth-child(2) {
      --text-delay: 1s;
    }

    &:nth-child(3) {
      --text-delay: 1.5s;
    }

    &:nth-child(4) {
      --text-delay: 2s;
    }

    &:nth-child(5) {
      --text-delay: 2.5s;
    }

    &:nth-child(6) {
      --text-delay: 3s;
    }
  }
}

@keyframes pulse-spread {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 0.3;
  }
}

@media screen and (min-width: 426px) and (max-width: 768px) {
  aside {
    margin-left: 40px;
    padding: 0 2.4rem 0 0;
  }
}

@media screen and (max-width: 425px) {
  aside {
    padding: 0 1rem;
  }

  .container {
    height: 100%;
  }

  .binary-text-svg {
    top: 50%;
    left: 0;
    bottom: 0;
  }
}
</style>
