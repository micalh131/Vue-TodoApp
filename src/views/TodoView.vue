<template>
  <div>
    <list-tasks v-if="$store.state.tasks.length" />
    <no-tasks v-else />
  </div>
</template>

<script>
import ListTasks from "@/components/Todo/ListTasks.vue";
import NoTasks from "@/components/Todo/NoTasks.vue";

export default {
  name: "Home",
  components: {
    "list-tasks": ListTasks,
    "no-tasks": NoTasks,
  },
};
</script>
