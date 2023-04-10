<script lang="ts">
	import { onMount } from "svelte";

  onMount(async() => {
    const eyes =[...document.querySelectorAll(".eyes span")] as HTMLSpanElement[]
  })
</script>



<div class="container">
  <span class="text">
    Vous avez un beau
projet ? parlons-en
autour d'un Bon café
  </span>

 
<div class="body">
  <div class="eyes">
    <span class="eye"></span>
    <span class="eye"></span>
  </div>
  <span class="mouth"></span>
</div>
</div>

<style lang="scss">
  .container {
    margin-top: 7vw;
    // padding: 5vw;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 70px;
  }
  
  .text {
    font-size: 4vw;
    width: 100dvw;
    text-align: center;
    font-family: var(--headline-font);
  }

  .body {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 150px;
  width: 150px;
  border-radius: 100px;
  border: 1px solid #fff;
  padding: 10x;
  gap: 20px;

}

.eyes {
  display: flex;
  width: 100%;
  display: flex;
  justify-content: space-around;
  padding: 0 10px;

  span {
    height: 20px;
    width: 15px;
    background-color: #fff;
    border-radius: 50%;
    
  }
  
}

.mouth {
  width: 50px;
  height: 40px;
  border-radius: 20px;
  border-bottom: 1px solid #fff;
  
}
</style>

