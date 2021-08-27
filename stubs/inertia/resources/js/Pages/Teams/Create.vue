<template>
  <app-layout title="Create Team">
    <template #header>
      <h2 class="h4 font-weight-bold">
          Create Team
      </h2>
    </template>

    <create-team-form />
    </app-layout>
</template>

<script>
    import AppLayout from '@/Layouts/AppLayout.vue'
    import CreateTeamForm from '@/Pages/Teams/Partials/CreateTeamForm.vue'

    export default {
        components: {
            AppLayout,
            CreateTeamForm,
        },
    }
</script>
