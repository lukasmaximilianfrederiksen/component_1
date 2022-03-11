<script>
</script>

<footer>
  <div class="grid-container">
    <div class="services">
      <h3>Services</h3>

      <ul>
        <li>
          <a href="">Branding</a>
          <a href="">Design</a>
          <a href="">Marketing</a>
          <a href="">Advertisment</a>
        </li>
      </ul>
    </div>

    <div class="company">
      <h3>Company</h3>

      <ul>
        <li>
          <a href="">About us</a>
          <a href="">Contact</a>
          <a href="">Jobs</a>
          <a href="">Press kit</a>
        </li>
      </ul>
    </div>

    <div class="legal">
      <h3>Legal</h3>

      <ul>
        <li>
          <a href="">Terms of use</a>
          <a href="">Privacy policy</a>
          <a href="">Cookie policy</a>
        </li>
      </ul>
    </div>
  </div>
</footer>

<style>
  footer {
    background: var(--footer-bg-color);
  }

  .grid-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
    justify-items: center;
  }

  ul {
    padding: 0;
  }
  li {
    list-style: none;
    text-align: left;
  }

  a {
    display: block;
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
    color: var(--font-color);
  }
</style>
