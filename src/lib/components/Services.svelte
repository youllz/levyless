<section>

  <div class="links">
    <span>
      <a href="/">DEJEUNER D'AFFAIRE</a>
    </span>
    <span>
      <a href="/">CANTINE</a>
    </span>
    <span>
      <a href="/">CEREMONIE</a>
    </span>
  </div>

  <div class="text">
    <p>
      grâce à un Storytelling <br>

impactant une identité <br>

visuelle forte des interfaces <br>

digitales ultra fluides <br>
    </p>
  </div>
  
</section>

<style lang="scss">
  section {
    width: 100dvw;
    height: 100%;
    padding-top: 7vw;
    overflow: hidden;
  }

  .links {
    width: 100%;
    display: flex;
    flex-direction: column;
  }

  span {
    width: 100%;
    font-size: 10vw;
    position: relative;

    a {
      font-family: var(--para-font);

      &::before {
        content: "";
        display: block;
        position: absolute;
        bottom: -1px;
        width: 100%;
        height: 2px;
        background-color: #fff;
      }
    }
  }

  .text {
    margin: 5vw;

    p {
      line-height: 1;
    }
  }
</style>