<template>
   <div>
       <h2>List of questions rendered here</h2>
       <question></question>
       <ul></ul>
   </div>
  
</template>

<script>
import Question from './Question.vue'; 
export default {
    name: 'list-of-questions',
    props: ['edin-questions-list'],
    components: {
        "question": Question
    }
    

}
</script>

<style scoped>

</style>