<nav>


 <div class="nav-container">
  <div class="social">
    <h4>SOCIAL</h4>
    <div class="social-links">
      <a href="/">Facebook</a>
      <a href="/">Whatsapp</a>
      <a href="/">Instagram</a>
    </div>
  </div>
  <div class="menu">
    <h4>MENU</h4>
    <div class="menu-links">
      <a href="/">Acceuil</a>
      <a href="/">Services</a>
      <a href="/">Gallerie</a>
      <a href="/">Contacts</a>
    </div>
  </div>
 </div>

 
  
</nav>



<style lang="scss">
  nav {
    width: 50vw;
    height: 100vh;
    background-color: #fff;
    color: #000;
    display: flex;
    flex-direction: column;
    position: fixed;
    right: 0;
    padding: 8rem 5vw 2rem;

  }

  .nav-container {
    display: flex;
    gap: 15vw;
  }

  h4 {
    color: var(--paragraph);
  }

  .menu{
    
    div {
      font-size: clamp(2rem, 10vw, 50px);
    }
  }

  .social, .menu {

    display: flex;
    flex-direction: column;
    gap: 40px ;

    div {
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    
    
    a {
      color: #000;
      
    }

  }
</style>