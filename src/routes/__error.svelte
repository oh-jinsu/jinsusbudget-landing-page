<script context="module">
  export function load({ _, status }) {
    return {
      props: {
        status,
      }
    }
  }
</script>

<script>
  export let status

  const message = status === 404
    ? "페이지를 찾지 못했습니다."
    : "예기치 못한 오류가 발생했습니다."
</script>

<section>
  <h2>{ message }</h2>
</section>

<style>
  section {
    padding: 16px 0;
  }
</style>