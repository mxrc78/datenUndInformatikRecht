<script setup>
import { ref } from 'vue'
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'

import HomeView from './views/HomeView.vue'
import FeaturesView from './views/FeaturesView.vue'
import DownloadView from './views/DownloadView.vue'
import AboutView from './views/AboutView.vue'
import LicenseView from './views/LicenseView.vue'
import PrivacyView from './views/PrivacyView.vue'
import ContactView from './views/ContactView.vue'
import ImprintView from './views/ImprintView.vue'
import AccessibilityView from './views/AccessibilityView.vue'

const currentPage = ref('home')

const pages = {
  home: HomeView,
  features: FeaturesView,
  download: DownloadView,
  about: AboutView,
  license: LicenseView,
  privacy: PrivacyView,
  contact: ContactView,
  imprint: ImprintView,
  accessibility: AccessibilityView
}
</script>

<template>
  <Navbar @navigate="currentPage = $event" />
  <main id="main-content">
    <component :is="pages[currentPage]" @navigate="currentPage = $event" />
  </main>
  <Footer @navigate="currentPage = $event" />
</template>