
<div class="body">
  <div class="eyes">
    <span></span>
    <span></span>
  </div>
  <span class="mouth"></span>
</div>



<style lang="scss">
.body {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100px;
  width: 100px;
  border-radius: 100px;
  border: 1px solid #fff;
  padding: 10x;
  gap: 20px;

}

.eyes {
  display: flex;
  width: 100%;
  display: flex;
  justify-content: space-between;
  padding: 0 10px;

  span {
    height: 20px;
    width: 15px;
    background-color: #fff;
    border-radius: 50%;
    
  }
  
}

.mouth {
  width: 40px;
  height: 20px;
  border-radius: 20px;
  border-bottom: 1px solid #fff;
  // border-bottom-left-radius: 50px;
  // border-bottom-right-radius: 50px;
}
</style>