<script>
import AppIcon from "src/components/app_icon.svelte";
import BadgeDownloadApple from "src/components/badge_download_apple.svelte";
import BadgeDownloadGoogle from "src/components/badge_download_google.svelte";

</script>
<svelte:head>
  <title>진수의 가계부</title>
</svelte:head>

<main>
  <section>
    <header>
      <AppIcon />
      <h1>진수의 가계부</h1>
    </header>
    <h2>하루에 얼마를 쓸까요?</h2>
    <p>
      너무 거창하게 시작하지 마세요. 딱 하루치 예산을 계획할 수 있습니다.
      <br />
      매일 진수의 가계부에 지출한 내역을 기록하세요.
      <br />
      남은 돈은 저금해 드립니다.
    </p>
    <div class="badge-container">
      <a class="apple" href="https://apps.apple.com/kr/app/%EC%A7%84%EC%88%98%EC%9D%98-%EA%B0%80%EA%B3%84%EB%B6%80/id1614177059?l=en" target="_blank">
        <BadgeDownloadApple />
      </a>
      <a class="google" href="https://play.google.com/store/apps/details?id=com.codersproduct.jinsusbudget">
        <BadgeDownloadGoogle />
      </a>
    </div>
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

  header {
    display: flex;

    align-items: flex-end;
  }

  h1 {
    margin-bottom: 12px;

    margin-left: 4px;
  }

  h2 {
    font-size: 72px;
  }

  p {
    margin-top: 8px;
    
    font-size: 18px;
  }

  .badge-container {
    display: flex;

    align-items: center;
  }

  @media (max-width: 480px) {
    h2 {
      margin-top: 4px;

      font-size: 40px;
    }

    p {
      margin-left: 2px;
    }

    .badge-container {
      margin-top: 32px;

      flex-direction: column;

      gap: 4px;
    }
  }

  @media (min-width: 481px) {
    h1 {
      font-size: 32px;
    }

    h2 {
      margin-left: 10px;
    }

    p {
      margin-left: 14px;
    }

    .badge-container {
      margin-top: 12px;

      margin-left: 10px;

      gap: 8px;
    }
  }
</style>
