<template>
  <section>
    <div class="container">
      <div class="card" v-for="person in people" :key="person.name">
        <div class="top">
          <img src="../assets/UserAvatar.svg" alt="" />
          <div class="title">
            <p class="name">{{ person.name + " " + person.surname }}</p>
            <p class="rev">{{ person.rev }}</p>
          </div>
        </div>
        <p class="para">
          {{ person.paragraph }}
        </p>

        <button>View {{ person.name }}'s Portfolio</button>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  data() {
    return {
      people: [
        {
          img: "",
          name: `Sarah`,
          surname: `Andrews`,
          rev: `100k`,
          paragraph: `Setting up my portfolio with Fiber took no more than 10 minutes. Since
          then, my portfolio has attracted a lot of clients and made me more
          than $100k`,
        },
        {
          img: "",
          name: `Matthew`,
          surname: `Higgins`,
          rev: `20k`,
          paragraph: `I have been getting A LOT of leads ever since I used Fiber's premade templates, now I just need to work on my case studies and I'll be ready to go!`,
            },
             {
          img: "",
          name: `Janica`,
          surname: `Dave`,
          rev: `30k`,
          paragraph: `I only started freelancing this year and I have already made more than I ever dreamed of in my full-time job.The templates are so amazing`,
            },
             {
          img: "",
          name: `Benjamin`,
          surname: `Wallace`,
          rev: `150k`,
          paragraph: `I only started freelancing this year and I have already made more than I ever dreamed of in my full-time job.The templates are so amazing`,
            }
        ],
    };
  },
};
</script>
<style scoped>
section {
  width: 100%;
  height: fit-content;
  display: flex;
  justify-content: flex-end;
  margin-top: 6rem;
  padding-bottom: 10rem;
}
.container {
  overflow-x: scroll;

  width: 90%;
  height: 21rem;
  display: flex;
  column-gap: 3rem;
}
.container::-webkit-scrollbar {
  display: none;
}
.card {
  border: 2px solid var(--lgrey);
  height: 100%;
  min-width: 27rem;
  width: 27rem;
  border-radius: 12px;
  display: flex;
  flex-direction: column;
  padding: 2rem;
  justify-content: space-between;
}
.top {
  display: flex;
  column-gap: 1rem;
  width: 100%;
}
.name {
  color: var(--blue);
  font-weight: 700;
}
.rev::after {
  content: " in revenue";
}
.para {
  font-size: 1.1rem;
  font-weight: 450;
}
button {
  padding-block: 1rem;
  border: 2px solid var(--lgrey);
  background: none;
  outline: none;
  border-radius: 6px;
  font-size: 1.2rem;
  font-weight: 700;
  color: var(--blue);
  transition: ease all .2s
}
button:hover{
    scale: 0.98;
}
img {
  width: 50px;
  height: auto;
  border-radius: 50%;
}
</style>
