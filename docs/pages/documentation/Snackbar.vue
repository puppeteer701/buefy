<template>
    <div>
        <h1 class="title is-spaced">Snackbar</h1>
        <h2 class="subtitle">When a Dialog seems a bit overkill for the task, Snackbars are good candidates</h2>
        <hr>

        <div class="block">
            <p>They can only have one button, and are queued to not confuse the user.</p>
            <p class="content"><small><b>Note:</b> They queue with <router-link to="/documentation/toast">Toasts</router-link> as well.</small></p>
        </div>

        <div class="block">
            <ex-simple></ex-simple>
        </div>
        <CodeView :code="ExSimpleCode" />

        <hr>
        <h2 class="title is-spaced">API</h2>
        <ApiView :data="api" />
    </div>
</template>

<script>
    import api from '@/apis/apiSnackbar'

    import ExSimple from '@/examples/snackbar/ExSimple'
    import ExSimpleCode from '!!raw-loader!@/examples/snackbar/ExSimple'

    export default {
        components: {
            ExSimple
        },
        data() {
            return {
                api,
                ExSimpleCode
            }
        }
    }
</script>
