<script>
    import '../../styles/components/auth/AuthForm.scss';
    import AuthButton from './AuthButton.vue';

    export default {
        components: {
            AuthButton: AuthButton
        }
    }
</script>

<template>
    <form method="POST" class="login-form">
        <section class="login-form__body">
            <fieldset class="login-form__body__inputs">
                <legend class="login-form__body__inputs__title">Логин</legend>
                <input 
                    class="login-form__body__inputs__input" 
                    type="text" 
                    placeholder="Введите логин">

                <legend class="login-form__body__inputs__title">Пароль</legend>
                <input 
                    class="login-form__body__inputs__input" 
                    type="text" 
                    placeholder="Введите пароль">
            </fieldset>
            <section class="login-form__body__actions">
                <RouterLink 
                    class="login-form__body__actions__link" 
                    to="/registration">Создать аккаунт</RouterLink>
                <RouterLink 
                    class="login-form__body__actions__link" 
                    to="/">Забыли пароль?</RouterLink>
            </section>
        </section>
        <section class="login-form__actions">
            <AuthButton label="Войти"/>
            <RouterLink class="login-form__actions__redirect" to="/">На главную</RouterLink>
        </section>
    </form>
</template>