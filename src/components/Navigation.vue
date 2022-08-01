<template>
  <div class="container">
    <nav class="nav-content">
      <img
        src="../assets/images/Logo.png"
        class="nav-logo"
        alt="Rez logo"
        width="150px"
        height="100px"
      />
      <ul class="nav-links">
        <li><a href="#">Home</a></li>
        <li><a href="#">Main</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  animation: fadeInAnimation ease 2s;
  animation-iteration-count: 1;
  animation-fill-mode: forwards;
}

@keyframes fadeInAnimation {
  0% {
    opacity: 0;
    transform: translateY(-80px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

.nav-logo {
  transform: translateY(30%);
}

.nav-content {
  align-items: flex-end;
  border: 3px solid rgba(164, 161, 161, 0.588);
  border-top: none;
  display: flex;
  justify-content: space-between;
  padding: 0 1rem;
  width: 60%;
}

.nav-links {
  display: flex;
}

li {
  list-style: none;
  margin: 0 1rem;
}

li:active {
  transform: scale(0.95);
  transition: 0.1s ease-in-out;
}

a {
  color: rgb(164, 161, 161);
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  text-decoration: none;
}

a:hover {
  color: white;
  transition: 0.2s ease-in-out;
}

a:active {
  color: gold;
  transition: 0.1s ease-in-out;
}

a:focus {
  border-bottom: 3px solid gold;
  padding-bottom: 1.2rem;
  transition: 0.1s ease-in-out;
}
</style>
