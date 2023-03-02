<template>
    <header class="header">
        <nav>
          <ul>
            <li>
              <router-link to="/">Home</router-link>
            </li>
            <li><router-link to="/counter">Counter</router-link></li>
          </ul>
        </nav>
        <section class="wrapper__main">
            <section class="home_page">
                <div class="text">
                    <h1>A Simple Counter App </h1>
                    <p>Made with vuejs</p>
                </div>
                <router-link to="/counter" class="a">start</router-link>
                <!-- <button class="__btn">start</button> -->
            </section>
        </section>
        
    </header>
    
    
    <section class="features">
        <h2>Features</h2>
        <div class="text__features">
            <h4>This counter App was created for the purpose of making counts with the use of increment,decrement, reset and setValue functions. The app is of great UI and was created with Vue js. <br>Project by Ononobi Favour✨..
            <br><button class="github">
                <a href="https://github.com/OnonobiFavour">GitHub repo</a>
            </button>
            </h4>
        </div>
        
    </section>
</template>

<style scoped>
    
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100vw;
}

nav ul {
  list-style: none;
  display: flex;
}

nav ul li {
  margin: 0 1rem;
}

nav ul li a {
  text-decoration: none;
  color: #ffff;
  font-size: 2.2rem;
  font-weight: bold;
}

nav ul li a:hover {
  text-decoration: underline;
}
.wrapper__main{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 100%;        
}
.header{
    width: 100vw;
    height: 100%;
    clip-path: ellipse(100% 55% at 44% 37%);
    background: linear-gradient(to right,rgb(228, 70, 97), rgb(193, 46, 75) ); 
}
.home_page{
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    max-width: 500px;
    animation-name: home-textBox;
    animation-duration: 2s;
    animation-iteration-count: 2s;
    height: 500px;
    align-items: center;
    justify-content: center;
    
}
@keyframes home-textBox{
    from{
        opacity: 0.5;
        transform: translateY(100%);
    }
    to{
        opacity: 1;
        transform: translateY(0%);
    }
}
h1{
    font-size: 40px;
    letter-spacing: 0.2rem;
}
p{
    font-size: 20px;
    padding: 1rem 0rem;
}
.text{
    text-align: center;
    color: white;
}
.a{
    color: #fff;
    text-decoration: none;
    font-weight: bolder;
    padding-top: 8px;
    width: 150px;
    text-align: center;
    height: 40px;
    font-size: 20px;
    background: inherit;
    border: 1px solid white;
    border-radius: 10px;
}
.a:hover{
    color: rgb(228, 70, 97);
    background-color: #fff;
    transition: 0.4s;
}
.features{
    position: absolute;
    max-width: 1000px;
    left: 7%;
    transform: translate(-50% 50%);
}
.text__features{
    font-size: 20px;
    max-width: 100%;
    height: 200px;
    padding: 1rem;
    color: grey;
}
h2{
    font-size: 40px;
    text-align: center;
}
h4{
    text-align: center;
}
.github{
    background-color: rgb(228, 70, 97);
    padding-left: 0.4rem;
    width: 250px;
    height: 40px;
    border-radius: 20px;
    margin: 2rem 0rem;
    border: none;
}
.github a{
    color: white;
    font-size: 20px;
    text-decoration: none;
}

</style>