<template>
  <!-- <HelloWorld /> -->

  <br>
  <v-table density="compact">
    <tbody>
      <tr v-for="(item, index)  of members" :key="`${index}-member`">
        <td>
          <img class="avatar" :src="item.img" alt="avatar">
        </td>
        <td>
          <div class="major-2">{{ item.name }}</div>
        </td>
        <td :style="item.status ? '' : 'padding:0'">
          {{ item.status }}
        </td>
        <td>
          <v-btn v-if="item.github" icon :href="item.github" target="_blank" size="x-small" variant="tonal">
            <v-icon icon="mdi-github"></v-icon>
          </v-btn>
          &nbsp;
          <v-btn v-if="item.linkedin" icon :href="item.linkedin" target="_blank" size="x-small" variant="tonal">
            <v-icon icon="mdi-linkedin"></v-icon>
          </v-btn>
          &nbsp;
          <v-btn v-if="item.instagram" icon :href="item.instagram" target="_blank" size="x-small" variant="tonal">
            <v-icon icon="mdi-instagram"></v-icon>
          </v-btn>
        </td>
      </tr>
    </tbody>
  </v-table>
</template>

<script setup>
// import HelloWorld from '@/components/HelloWorld.vue'
const members = [
  {
    id: 1,
    name: 'Vitaliy Dyachuk',
    img: 'https://avatars3.githubusercontent.com/u/16016599?s=460&v=4',
    status: 'CLAN-leader, super-mentor',
    carma: 1000,
    level: 0,
    github: 'https://github.com/SpiritUrban',
    linkedin: 'https://www.linkedin.com/in/vitaly-dyachuk-8ba18a54/',
    instagram: 'https://www.instagram.com/shadespiritenator/'
  },
  {
    id: 11,
    name: 'Diana',
    img: 'https://avatars.githubusercontent.com/u/113860914?v=4',
    status: 'student',
    carma: 100,
    level: 0,
    github: 'https://github.com/NedVlor',
    linkedin: '',
    instagram: ''
  },
  {
    id: 2,
    name: 'Roman Peredrii',
    img: 'https://avatars0.githubusercontent.com/u/42037680?s=460&v=4',
    status: 'student, mentor',
    carma: 100,
    level: 0,
    github: 'https://github.com/RomanPeredrii',
    linkedin: '',
    instagram: ''
  },
  {
    id: 3,
    name: 'Vladyslav Piatyhor',
    img: 'https://avatars1.githubusercontent.com/u/29441499?s=460&v=4',
    status: 'student',
    carma: 100,
    level: 0,
    github: 'https://github.com/5Mountains',
    linkedin: '',
    instagram: ''
  },
  {
    id: 4,
    name: 'Taras Ostasha',
    img: 'https://avatars3.githubusercontent.com/u/19312196?s=460&v=4',
    status: 'student',
    carma: 100,
    level: 0,
    github: 'https://github.com/TarasOstasha',
    linkedin: '',
    instagram: ''
  },
  {
    id: 5,
    name: 'Vlad Buryak',
    img: 'assets/img/base/icons/avatars/batman.svg',
    status: 'student',
    carma: 100,
    level: 0,
    github: 'https://github.com/VladGodOfJS',
    linkedin: '',
    instagram: ''
  },
  {
    id: 6,
    name: 'Oksana Soroka',
    img: 'assets/img/base/icons/avatars/woman.svg',
    status: 'student',
    carma: 100,
    level: 0,
    github: '',
    linkedin: 'http://linkedin.com/in/oksana-soroka-45282919a',
    instagram: 'https://www.instagram.com/ksu_mid/'
  },
  {
    id: 7,
    name: 'Kolya (Toto)',
    img: 'https://avatars3.githubusercontent.com/u/33295757?s=460&v=4',
    status: 'student',
    carma: 100,
    level: 0,
    github: 'https://github.com/Mooninghnk',
    linkedin: '',
    instagram: ''
  },

  {
    id: 8,
    name: 'Sergiy Semeguk',
    img: 'https://avatars2.githubusercontent.com/u/45179731?s=460&v=4',
    status: 'student',
    carma: 100,
    level: 0,
    github: 'https://github.com/semeguk',
    linkedin: '',
    instagram: ''
  },
  {
    id: 9,
    name: 'Dima Semeguk',
    img: 'https://avatars1.githubusercontent.com/u/51905745?s=460&v=4',
    status: 'student',
    carma: 100,
    level: 0,
    github: 'https://github.com/dimasemehuk7',
    linkedin: '',
    instagram: ''
  },
  {
    id: 10,
    name: 'Dima Martinovich',
    img: 'https://avatars.githubusercontent.com/u/47226234?v=4',
    status: 'student',
    carma: 100,
    level: 0,
    github: 'https://github.com/marpusik',
    linkedin: 'https://www.linkedin.com/in/%D0%B4%D0%B8%D0%BC%D0%B0-%D0%BC%D0%B0%D1%80%D1%82%D0%B8%D0%BD%D0%BE%D0%B2%D0%B8%D1%87-0881a5196/',
    instagram: ''
  }
]
</script>

<style>
.avatar {
  width: 2rem;
  border-radius: 2rem;
}
</style>