<template>
  <section>
    <div class="container">
      <div class="card" v-for="person in people" :key="person.name">
        <div class="top">
          <img :src="person.img" alt="" />
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
          img: "https://raw.githubusercontent.com/0xjoshva/fiber-webpage/211d2e90d0c55f39e94ecfa54484a8ffdc85f1ce/src/assets/UserAvatar.svg",
          name: `Sarah`,
          surname: `Andrews`,
          rev: `100k`,
          paragraph: `Setting up my portfolio with Fiber took no more than 10 minutes. Since
          then, my portfolio has attracted a lot of clients and made me more
          than $100k`,
        },
        {
          img: "https://raw.githubusercontent.com/0xjoshva/fiber-webpage/211d2e90d0c55f39e94ecfa54484a8ffdc85f1ce/src/assets/UserAvatar-2.svg",
          name: `Matthew`,
          surname: `Higgins`,
          rev: `20k`,
          paragraph: `I have been getting A LOT of leads ever since I used Fiber's premade templates, now I just need to work on my case studies and I'll be ready to go!`,
            },
             {
          img: "https://raw.githubusercontent.com/0xjoshva/fiber-webpage/211d2e90d0c55f39e94ecfa54484a8ffdc85f1ce/src/assets/UserAvatar3.svg",
          name: `Janica`,
          surname: `Dave`,
          rev: `30k`,
          paragraph: `I only started freelancing this year and I have already made more than I ever dreamed of in my full-time job.The templates are so amazing`,
            },
             {
          img: "data:image/jpeg;base64,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",
          name: `Benjamin`,
          surname: `Wallace`,
          rev: `150k`,
          paragraph: `I only started freelancing this year and I have already made more than I ever dreamed of in my full-time job.The templates are so amazing`,
            },
              {
          img: "https://pulse.seattlechildrens.org/wp-content/uploads/Person_Hannibal-001-700x467.jpg",
          name: `Peter`,
          surname: `Davidson`,
          rev: `75k`,
          paragraph: `I only started freelancing this year and I have already made more than I ever dreamed of in my full-time job.The templates are so amazing`,
            },
            {
          img: "https://members-api.parliament.uk/api/Members/2486/Portrait?cropType=OneOne",
          name: `Shelly`,
          surname: `Wrigleys`,
          rev: `15k`,
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
  scroll-snap-type: x proximity;
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
  scroll-snap-align: start;
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
  object-fit: cover;
  object-position: center;
}
</style>
