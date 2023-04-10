<script lang="ts">
	import Nav from '$lib/components/Nav.svelte';
  import '../style/app.scss'
</script>

<!-- <Nav/> -->
<header>
  <strong>
    LEVYLESS
  </strong>


  <div>
    <span>
      menu
    </span>
    <button>
      <span></span>
      <span></span>
      <span></span>
    </button>
  </div>
</header>

<main>
  <slot/>
</main>


<style lang="scss">
  header {
    width: 100dvw;
    display: flex;
    padding: 30px;
    justify-content: space-between;
    position: fixed;
    mix-blend-mode: difference;
    z-index: 100;

    strong {
      font-family: var(--highlight-font);
    }
    
    button {
      
      background: transparent;
      outline: none;
      border: none;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      gap: 5px;
      cursor: pointer;


      span {
        background-color: var(--headline);
        width: 30px;
        height: 2px;
      }

      
    }

    div {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 15px;

      span {
        font-family: var(--para-font);
      }
    }
  }

  main {
    height: 100%;
    width: 100dvw;
  }
</style>