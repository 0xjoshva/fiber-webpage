<template>
  <section>
    <div class="container">
      <div class="left">
        <div class="rating">
          <div class="stars">
            <img src="../assets/star.svg" alt="" />
            <img src="../assets/star.svg" alt="" />
            <img src="../assets/star.svg" alt="" />
            <img src="../assets/star.svg" alt="" />
            <img src="../assets/star.svg" alt="" />
          </div>
          <p>Rated 4.8/5 (243 reviews)</p>
        </div>
        <h1>Create your portfolio in minutes.</h1>
        <p>
          With Fiber, you can setup your own personal portfolio in minutes with
          dozens of premade, beautiful templates.
        </p>
        <div class="herobtn">
          <button>Start Free Trial</button>
          <button>View Examples</button>
        </div>
        <div class="checkdiv">
            <span class="check"><img src="../assets/Checkmark.svg" alt="" id="checkimg"> <p>No Credit Card Required</p></span>
            <span class="check"><img src="../assets/Checkmark.svg" alt="" id="checkimg"> <p>10 Free Templates</p></span>
        </div>
      </div>
      <img src="../assets/hero-Illustration.png" alt="" />
    </div>
  </section>
</template>
<script>
export default {};
</script>
<style scoped>
section {
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
}
.container {
  background: var(--white);
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: calc(100vh - 100px);
  width: 80%;
  height: fit-content;

}
img {
  width: 50%;
}
.left{
    width:50%;
    border:1px solid black;
    height: fit-content;
}
.stars {
  display: flex;
  column-gap: 0.3rem;
}
.rating {
  display: flex;
  align-items: center;
  width: fit-content;
  column-gap: 1.2rem;
font-size: 1.2rem;
font-weight: 500;
margin-bottom: .8rem;
}
.checkdiv{
    display: flex;
    width: 100%;
    column-gap: 1rem;
}
.check{
    display: flex;
    justify-content: center;
    align-items: center;
    width: fit-content;
    column-gap: .5rem;
}
#checkimg{
    width: 1.5rem;
    height: auto;
}
h1{
    font-size: 4.2rem;
    line-height: 4.8rem;
}
</style>
