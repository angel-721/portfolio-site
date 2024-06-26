<script>
  import selfImage from "../../../public/assets/images/angel_m_v.webp";
</script>

<div class="grid" style="margin-top: 2rem">
  <div id="name-div">
    <h3>Welcome! My name is:</h3>
    <h1 id="my-name">Angel Velasquez</h1>
    <img src={selfImage.src} alt="Angel Velasquez" decoding="async" />
  </div>

  <p id="bio">
    I'm a rising master's student at Lehigh University studying Computer
    Science. I'm passionate about data science, machine learning, and game
    development.
  </p>
</div>

<style lang="CSS">
  #name-div h3 {
    color: whitesmoke;
  }

  #name-div h1 {
    margin-top: -0.8rem;
    margin-left: 4rem;
  }

  img {
    width: 256px;
	height: auto;
    margin: 10px;
    border: 2px solid whitesmoke;
    border-radius: 500px;
    -webkit-border-radius: 500px;
    -moz-border-radius: 500px;
  }

  @keyframes fadeIn {
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }

  #my-name {
    animation: fadeIn 1s;
  }

  #bio {
    font-size: 1.5rem;
  }
</style>
