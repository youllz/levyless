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
    <video src="https://media.wearemotto.com/app/uploads/2022/11/14104333/home-hero-opt.mp4" muted loop preload="metadata" autoplay></video>
  </figure>
</section>
<section class="hero-sub-text">
  <h1>
      nous 
   sommes la pour <span> APPORTER DU BONHEUR</span> dans   <span>VOS ASSIETE</span>
  </h1>
</section>


<style lang="scss">
  .hero-text {
    width: 100dvw;
    padding: 5vw;
    padding-top: clamp(9rem, 0vw, 180px);
    
    height: 100%;
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
    padding-top: 7vw;
    height: 150vh;
    width: 100dvw;

    figure {
      height: 40%;
      width: 40%;
      position: sticky;
      top: 0;


      video {
        height: 100%;
        width: 100%;
      }
    }
  }

  .hero-sub-text{
    width: 100dvw;
    height: 100vh;
    padding: 5vw;
    overflow: hidden;

    h1 {
      font-size: 9vw;

      span {
        font-family: var(--highlight-font);
      }
    }
  }

</style>