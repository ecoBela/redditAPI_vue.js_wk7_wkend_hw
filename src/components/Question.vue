<template>
    <div>
        <li>Individual question rendered here</li>
        <question-details></question-details>
    </div>
  
</template>

<script>
import QuestionDetails from './QuestionDetails.vue';
export default {
    name: 'question',
    components: {
        "question-details": QuestionDetails
    }

}
</script>

<style scoped>

</style>