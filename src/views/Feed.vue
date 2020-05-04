<template>
  <div class="pa-2 px-sm-8 py-sm-4 ">
    <QuestionsCard :title="false" divider></QuestionsCard>
  </div>
</template>
<script>
    import QuestionsCard from "../components/questions/QuestionsCard";
    export default {
        name: 'Feed',
        components: {
            QuestionsCard
        }
    }
</script>
