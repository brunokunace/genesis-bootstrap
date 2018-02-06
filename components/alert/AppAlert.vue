<template>
    <div>
        <b-alert v-bind="{show, variant, dismissible, dismissLabel}">
            <slot/>
        </b-alert>
    </div>
</template>

<script>
    export default {
        extends: {},
        mixins: [],
        name: 'AppAlertBootstrap',
        props: {
            show: {
                type: [Boolean, Number],
                default: () => false
            },
            variant: {
                type: String,
                default: () => 'info'
            },
            dismissible: {
                type: Boolean,
                default: () => false
            },
            dismissLabel: {
                type: String,
                default: () => 'Close'
            },
        }
    }
</script>