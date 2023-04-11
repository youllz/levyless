<script lang="ts">
	import { onMount } from "svelte";

  onMount(async() => {
    const eyes =[...document.querySelectorAll(".eye")] as HTMLSpanElement[]
    // const anchor = document.querySelector('.body') as HTMLDivElement

    window.addEventListener('mousemove', (event:MouseEvent) => {
      const mouseX = event.clientX * 100 /window.innerWidth + '%'
      const mouseY = event.clientY * 100 / window.innerHeight + '%'

      eyes.forEach(eye => {
        eye.style.left = mouseX
        eye.style.top = mouseY

        eye.style.transform = "translate( -" + mouseX + ",-" + mouseY + ")"
      })

    })

   
  })
</script>



<div class="container">
  <span class="text">
    Vous avez un beau
projet ? parlons-en
autour d'un Bon café
  </span>

 
<div class="body">
  <div class="eyes-container">
    <div class="eyes">
      <span class="eye"></span>
    </div>
    <div class="eyes">
      <span class="eye"></span>
    </div>
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
  height: 200px;
  width: 200px;
  border-radius: 100px;
  border: 1px solid #fff;
  padding: 10x;
  gap: 20px;

}

.eyes-container {
  display: flex;
  gap: 30px;
  align-items: center;
}

.eyes {
  display: flex;
  width: 100%;
  display: flex;
  justify-content: space-around;
  padding: 0 10px;
  position: relative;
  height: 50px;
  width: 30px;
  border-radius: 50%;
  border: 1px solid #fff;
  overflow: hidden;

  span {
    height: 20px;
    width: 15px;
    background-color: #fff;
    border-radius: 50%;
    position: absolute;
    
  }
  
}

.mouth {
  width: 50px;
  height: 40px;
  border-radius: 20px;
  border-bottom: 1px solid #fff;
  
}
</style>

