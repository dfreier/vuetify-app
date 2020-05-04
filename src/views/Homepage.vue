<template>
  <div class="pa-2 px-sm-8 py-sm-4 ">
    <QuestionsCard title="Questions for you" icon="mdi-star-four-points-outline"></QuestionsCard>
    <Subscriptions></Subscriptions>
  </div>
</template>

<script>
    import QuestionsCard from "../components/questions/QuestionsCard";
    import Subscriptions from "../components/homepage/Subscriptions";

    export default {
        name: 'HelloWorld',
        components: {
            QuestionsCard,
            Subscriptions
        }
    }
</script>
