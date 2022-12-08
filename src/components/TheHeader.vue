<template>
  <header class="container">
    <div class="header">
      <div class="header__logo">
        <a href="../App.vue">
          <img src="../assets/icons/coozin_logo.svg" alt="coozin logo"/>
        </a>
      </div>
      <form class="header__form">
        <label class="header__icon" for="search">
          <img src="../assets/icons/address.svg" alt="search icon" />
        </label>
        <input id="search" type="text" placeholder="Можно узнать где ты?" />
      </form>
      <nav>
        <ul class="header__nav">
          <li class="header__nav-list"><a href="#"> Наша история</a></li>
          <li class="header__nav-list"><a href="#">Присоединиться</a></li>
          <li class="header__nav-list"><a href="#">Блог</a></li>
        </ul>
      </nav>
      <div class="header__buttons">
        <a href="#">
          <div class="header__icon orange">
            <img src="../assets/icons/Shopping.svg" alt="shopping icon" />
          </div>
        </a>
        <a href="#">
          <div class="header__icon">
            <h3 class="header__icon-h3">UZ</h3>
          </div>
        </a>
        <a href="#">
          <div class="header__icon">
            <img src="../assets/icons/User.svg" alt="user icon" />
          </div>
        </a>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "TheHeader",
};
</script>

<style scoped>
.header {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 16px 0px 20px;
}

.header__logo img {
  width: 150px;
  height: 36px;
}

.header__form {
  display: flex;
  gap: 12px;
  cursor: pointer;
}

.header__icon {
  width: 48px;
  height: 48px;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #f3f4f6;
  border-radius: 16px;
}

form label,
#search {
  cursor: pointer;
}

#search {
  width: 256px;
  border: 1px solid #e5e7eb;
  border-radius: 16px;
  background-image: url(../assets/icons/Location\ marker.svg);
  background-repeat: no-repeat;
  background-position-x: 16px;
  background-position-y: 9px;
  outline: none;
  padding-left: 44px;
}

.header__form:hover #search {
  border: 1px solid orangered;
}

::-webkit-input-placeholder {
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  color: #6b7280;
}

.header__nav {
  display: flex;
  gap: 48px;
}

.header__nav-list a {
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  color: #1f2937;
}

.header__nav-list {
  cursor: pointer;
  border-bottom: 6px solid transparent;
}
.header__nav-list:hover {
  border-bottom: 2.5px solid orangered;
  transform: translateY(1px);
}

.orange {
  background: #fff7ed;
}

.header__icon-h3 {
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  color: #1f2937;
}

.header__buttons {
  display: flex;
  gap: 16px;
}
</style>