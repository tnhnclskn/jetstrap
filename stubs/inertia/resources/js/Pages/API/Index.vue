<template>
    <app-layout title="API Tokens">
        <template #header>
            <h2 class="h4 font-weight-bold">
                API Tokens
            </h2>
        </template>

        <api-token-manager :tokens="tokens"
                           :available-permissions="availablePermissions"
                           :default-permissions="defaultPermissions" />
    </app-layout>
</template>

<script>
    import ApiTokenManager from '@/Pages/API/Partials/ApiTokenManager.vue'
    import AppLayout from '@/Layouts/AppLayout.vue'

    export default {
        props: [
            'tokens',
            'availablePermissions',
            'defaultPermissions',
        ],

        components: {
            ApiTokenManager,
            AppLayout
        },
    }
</script>
