<template>
  <div class="is-fluid is-gapless">
    <div class="columns">
      <div class="column is-2">
        <aside class="menu">
          <div class="side-menu-items">
            <p class="menu-label">
              Genaral
            </p>
            <ul class="menu-list">
              <li><a href="#">Dashboard</a></li>
            </ul>
            <p class="menu-label">Content Management</p>
            <ul class="menu-list">
              <li><a href="#">Crops</a></li>
              <li><a href="#">Category</a></li>
              <li><a href="#">Content</a></li>
              <li><a href="#">Menu Structure</a></li>
              <li><a href="#">Link Content</a></li>
              <li><a href="#">Notifications</a></li>
              <li><a href="#">Pricing</a></li>
            </ul>
            <p class="menu-label">
              Miscelenious
            </p>
            <ul class="menu-list">
              <li><a href="#">Agents</a></li>
              <li><a href="#">Suppliers</a></li>
              <li><a href="#">Reports</a></li>
              <li><a href="#">Reminders</a></li>
              <li><a href="#">Comments</a></li>
            </ul>
          </div>
        </aside>
      </div>
      <div class="column">
        <div class="tabs is-medium is-full1width">
          <ul>
            <li class="is-active">
              <a href="#">
                                <span class="icon is-small">
                                    <i class="fas fa-user-circle"></i>
                                </span>
                <span>Hello! Admin</span>
              </a>
            </li>
            <li>
              <a href="#">
                <span class="icon is-small"><i class="fas fa-home" aria-hidden="true"></i></span>
                <span>Home</span>
              </a>
            </li>
            <li>
              <a href="#">
                <span class="icon is-small"><i class="fas fa-info-circle" aria-hidden="true"></i></span>
                <span>About</span>
              </a>
            </li>
            <li>
              <a href="#">
                <span class="icon is-small"><i class="fas fa-sitemap" aria-hidden="true"></i></span>
                <span>Content</span>
              </a>
            </li>
            <li>
              <a href="#">
                <span class="icon is-small"><i class="fas fa-sign-out-alt" aria-hidden="true"></i></span>
                <span>Sign Out</span>
              </a>
            </li>
          </ul>
        </div>
        <nuxt/>
      </div>
    </div>
  </div>
</template>

<script>
  export default {}
</script>

<style>
  .menu {
    background-color: #19d88e;
  }

  .side-menu-items {
    padding: 2rem;
  }
</style>

