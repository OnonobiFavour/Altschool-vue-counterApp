<template>
    <nav>
      <ul>
        <li>
          <router-link to="/">Home</router-link>
        </li>
        <li><router-link to="/counter">Counter</router-link></li>
      </ul>
    </nav>
</template>
<style scoped>
nav {
  display: flex;
  justify-content: center;
  width: 100vw;
  align-items: center;
}

nav ul {
  list-style: none;
  display: flex;
}

nav ul li {
  margin-left:  1rem;
}

nav ul li a {
  text-decoration: none;
  color: rgb(238, 114, 135);
  font-size: 2.2rem;
  font-weight: bold;
}

nav ul li a:hover {
  text-decoration: underline;
}
</style>