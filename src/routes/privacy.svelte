<script>
import AppIcon from "src/components/app_icon.svelte";

</script>

<main>
  <section>
    <a href="/">
      <AppIcon />
    </a>

    <h1>진수의 가계부는 사용자의 개인 정보를 수집하지 않습니다.</h1>
  </section>
</main>

<style>
  main {
    display: flex;

    justify-content: center;

    align-items: center;

    width: 100%;

    min-height: 720px;

    background-color: #ffca28;
  }

  section {
    max-width: 768px;

    width: 100%;

    padding: 0 16px 48px 16px;
  }

  h1 {
    margin-top: 8px;
  }
</style>