<script lang="ts">
	import Emoji from "./Emoji.svelte";

let heroText = "SALUT"
</script>

<section class="hero-text">
  <h2>
    {#each heroText as letter}
      <span>{letter}</span>
    {/each}
  </h2>
  <!-- <Emoji/> -->
  <p>NOUS SOMMES  L'EQUIPE <span>LEVYLESS</span></p>
 
</section>
<section class="hero-video">
  <figure>

  </figure>
</section>


<style lang="scss">
  .hero-text {
    width: 100dvw;
    padding: 5vw;
    padding-top: clamp(9rem, 0vw, 180px);
    
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: flex-start;
    flex-direction: column;
    // background-color: red;
  }

 

  h2 {
    font-size: 28vw;
    font-weight: 800;
    letter-spacing: -.4vw;
    line-height: .9;
    text-align: center;
    // letter-spacing: 1.1px;
    display: flex;

    span {
      display: flex;
      align-items: center;
      justify-content: center;
    }
  }

  .hero-video {
    height: 100vh;
    width: 100dvw;
  }

</style>