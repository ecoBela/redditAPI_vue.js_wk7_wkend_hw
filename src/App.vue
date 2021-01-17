<template>
  <p>This is where the list component will appear</p>
</template>

<script>
export default {
  name: 'app',
  data(){
    return {
      edinburghQuestionsList: []

    }
  },
  mounted(){
    fetch('https://www.reddit.com/r/edinburgh.json')
    .then(res => res.json())
    .then(data => this.edinburghQuestionsList = data)
  },
  methods: {

  },
  
  components: {

  }

}
</script>

<style>

</style>