<script>
    import { link } from "svelte-routing";
</script>

<nav class="navbar navbar-expand-lg navbar-light bg-white p-3 px-4 fixed-top">
  <div class="container-fluid">
    <a class="navbar-brand" href="/" use:link>ALOMOVES</a>
    <button
      class="navbar-toggler"
      type="button"
      data-bs-toggle="collapse"
      data-bs-target="#navbarNavDropdown"
      aria-controls="navbarNavDropdown"
      aria-expanded="false"
      aria-label="Toggle navigation">
      <span class="navbar-toggler-icon" />
    </button>
    <div class="collapse navbar-collapse" id="navbarNavDropdown">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item">
          <a class="nav-link" href="/instructors" use:link>INSTRUCTORS</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/explores" use:link>EXPLORES</a>
        </li>
        <li class="nav-item dropdown dd-shop">
          <a class="nav-link navbar-shop-dropdown" href="#!">
            SHOP <div class="navbar-shop-badge" />
          </a>
          <div class="dropdown-menu dd-shop-menu">
            <a class="dropdown-item" href="#!">GEAR</a>
            <div class="dropdown-divider" />
            <a class="dropdown-item" href="#!">CLOTHING</a>
            <div class="dropdown-divider" />
            <a class="dropdown-item" href="#!">GIFT CARD</a>
          </div>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/login" use:link>SIGN IN</a>
        </li>
      </ul>
    </div>
  </div>
</nav>

<style>
  .navbar-shop-badge {
    display: inline-block;
    border-radius: 50%;
    background-color: rgb(198, 40, 40);
    position: relative;
    margin-left: 3px;
    padding: 4px;
  }
  .navbar-shop-dropdown::after {
    display: none;
  }
  .dd-shop:hover .dd-shop-menu {
      display:block;
  }
</style>
