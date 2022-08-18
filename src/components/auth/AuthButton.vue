<script>
    import '../../styles/components/auth/AuthButton.scss'
    export default {
    props: {
        label: String,
    }
}

</script>

<template>
    <button class="auth-button">
        {{ label }}
    </button>
</template>