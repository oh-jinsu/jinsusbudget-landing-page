<script>
  const year = new Date().getFullYear()
</script>

<footer>
  <div class="inner">
    <p>© { year } codersproduct.</p>
  </div>
</footer>

<style>
  footer {
    display: flex;

    justify-content: center;
    
    width: 100%;
  }

  .inner {
    max-width: var(--width-inner);

    width: 100%;

    padding: 16px;
  }
</style>