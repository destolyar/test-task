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
    <form method="POST" class="registration-form">
        <section class="registration-form__body">
            <fieldset class="registration-form__body__inputs">
                <legend class="registration-form__body__inputs__title">Логин</legend>
                <input 
                    class="registration-form__body__inputs__input" 
                    type="text" 
                    placeholder="Введите логин">
                
                <legend class="registration-form__body__inputs__title">E-mail адрес</legend>
                <input 
                    class="registration-form__body__inputs__input" 
                    type="text" 
                    placeholder="Введите E-mail">

                <legend class="registration-form__body__inputs__title">Пароль</legend>
                <input 
                    class="registration-form__body__inputs__input" 
                    type="text" 
                    placeholder="Введите пароль">
                
                <legend class="registration-form__body__inputs__title">Подтверждение пароля</legend>
                <input 
                    class="registration-form__body__inputs__input" 
                    type="text" 
                    placeholder="Повторите пароль">
            </fieldset>
        </section>
        <section class="registration-form__actions">
            <AuthButton label="Регистрация"/>
            <RouterLink 
                class="registration-form__actions__redirect" 
                to="/login">Уже есть аккаунт</RouterLink>
        </section>
    </form>
</template>