<template>
  <header>
    <b-navbar class="is-light">
      <template slot="start">
        <b-navbar-item tag="nuxt-link" to="/">Главная</b-navbar-item>
        <b-navbar-item tag="nuxt-link" to="/service">Сервис </b-navbar-item>
        <b-navbar-item tag="nuxt-link" to="/faq">FAQ </b-navbar-item>
      </template>

      <template slot="end">
        <b-navbar-item tag="div">
          <div class="signup-buttons">
            <b-button type="is-primary">
              <strong>Регистрация</strong>
            </b-button>
            <b-button type="is-link is-light">Логин</b-button>
          </div>
        </b-navbar-item>
      </template>
    </b-navbar>
  </header>
</template>

<script>
export default {}
</script>

<style></style>
