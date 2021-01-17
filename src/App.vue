<template>
   <div>
        <div>
            <list-of-questions></list-of-questions>
            <question-details></question-details>
        </div>
    </div>
</template>

<script>
import ListOfQuestions from './components/ListOfQuestions.vue';

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
    "list-of-questions": ListOfQuestions

  }

}
</script>

<style scoped>

</style>