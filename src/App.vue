<template>
<div id="app" class="container-fluid">
  <header>
    <nav class="navbar navbar-default">
      <div class="container-fluid">
        <div class="navbar-header">
          <a class="navbar-brand" href="#" id="logo">
            {{logo}}
          </a>
        </div>
        <p class="navbar-text navbar-right" style="margin-right:10px">
          Signed in as <a href="#" class="navbar-link"><u>Member</u></a>
          &nbsp;&nbsp;<span class="glyphicon glyphicon-arrow-right" aria-hidden="true"></span>
          <a href="#" class="navbar-link"><u>Sign Out</u></a>
        </p>
      </div>
    </nav>
  </header>
  <main>
    <ul class="nav nav-tabs" id="nav-tabs">
      <li role="presentation"><a href="#">HELP</a></li>
      <li role="presentation" class="active"><a href="#" style="background: #e8eaec">AGENTS</a></li>
      <li role="presentation"><a href="#">MY CRUICE</a></li>
      <li role="presentation"><a href="#">DASHBOARD</a></li>
    </ul>
    <agents-list></agents-list>
  </main>
  <footer>
    <p class="text-capitalize">copyright: thoughtworks.inc</p>
  </footer>
</div>
</template>

<script>
import AgentsList from './components/AgentsList.vue'

export default {
  name: 'App',
  data: function() {
    return {
      logo: 'Cruise'
    }
  },
  components: {
    AgentsList
  }
}
</script>

<style>
#nav-tabs.nav-tabs>li {
  float: right;
}
</style>
