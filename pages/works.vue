<template>
  <div class="Header">
    <page-header :header-item="headerItem">
      {{ title }}
    </page-header>
    <work-content />
  </div>
</template>

<script>
import PageHeader from '~/components/PageHeader.vue'
import WorkContent from '~/components/works/WorkContent.vue'

export default {
  components: {
    // eslint-disable-next-line vue/no-unused-components
    PageHeader,
    // eslint-disable-next-line vue/no-unused-components
    WorkContent
  },
  data() {
    const data = {
      title: 'TECHNOLOGY×ART2019 WORKS',
      headerItem: [
        {
          content: '2018',
          url: 'http://www.mono.eng.yamaguchi-u.ac.jp/Tech_Art/about/index.html'
        },
        {
          content: '2017',
          url: 'http://www.mono.eng.yamaguchi-u.ac.jp/garden/'
        },
        {
          content: '2016',
          url: 'http://www.mono.eng.yamaguchi-u.ac.jp/garden/index2.html'
        }
      ]
    }

    return data
  },
  head() {
    return {
      title: 'Technology×Art2019 作品集'
    }
  }
}
</script>

<style lang="scss" scoped>
/*
  .Header {
    display: flex;
    flex-wrap: wrap;
    align-items: flex-end;
  }
     */
</style>
