<template>
  <nav v-if="windowWidth >= 999" class="menu">
    <div
      v-for="(item, index) in menu"
      :key="index"
      :class="{
        'item--selected':
          categorySelected && categorySelected.name === item.name
      }"
      class="item"
      @click="selectCategory(index)"
    >
      <div class="item__label">{{ item.name }}</div>
      <div v-if="item.children" class="item__arrow"></div>
    </div>
    <transition name="fade">
      <div v-if="categorySelected" class="menu__dropdown dropdown">
        <div class="dropdown__overlay" @click="closeDropdown"></div>
        <div class="dropdown__wrapper">
          <div class="dropdown__children">
            <div
              v-for="(child, index) in categorySelected.children"
              :key="index"
              class="dropdown__child"
            >
              {{ child.name }}
            </div>
          </div>
          <div class="dropdown__posts">
            <div
              v-for="(item, index) in categorySelected.children"
              :key="index"
              class="post"
            >
              <img class="post__thumbnail" src="~/static/thumbnail.png" />
              <div class="post__footer">
                <div class="post__title">Welcome To The Machine</div>
                <div class="post__description">Antimatter singles</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </transition>
  </nav>
  <nav v-else class="menu-mobile"></nav>
</template>

<script>
export default {
  name: 'HeaderNavigationMenu',
  data() {
    return {
      windowWidth: 0,
      categorySelected: null,
      categoryPosts: null,
      menu: [
        {
          name: 'News',
          children: [
            { name: 'Food' },
            { name: 'Cinema' },
            { name: 'Lifehacks' },
            { name: 'Music' },
            { name: 'Travel' },
            { name: 'Family' },
            { name: 'TV' },
            { name: 'Tests' },
            { name: 'Humor' }
          ]
        },
        {
          name: 'Entertainment',
          children: [
            { name: 'Food' },
            { name: 'Cinema' },
            { name: 'Lifehacks' },
            { name: 'Music' },
            { name: 'Travel' },
            { name: 'Family' },
            { name: 'TV' },
            { name: 'Tests' },
            { name: 'Humor' }
          ]
        },
        {
          name: 'People',
          children: [
            { name: 'Food' },
            { name: 'Cinema' },
            { name: 'Lifehacks' },
            { name: 'Music' },
            { name: 'Travel' },
            { name: 'Family' },
            { name: 'TV' },
            { name: 'Tests' },
            { name: 'Humor' }
          ]
        },
        {
          name: 'More',
          children: [
            { name: 'Food' },
            { name: 'Cinema' },
            { name: 'Lifehacks' },
            { name: 'Music' },
            { name: 'Travel' },
            { name: 'Family' },
            { name: 'TV' },
            { name: 'Tests' },
            { name: 'Humor' }
          ]
        },
        { name: 'Your CHOIZ', children: false }
      ]
    }
  },
  mounted() {
    window.addEventListener('resize', this.updateWidth)
    this.updateWidth()
  },
  methods: {
    updateWidth() {
      this.windowWidth = window.innerWidth
    },
    selectCategory(index) {
      if (!this.menu[index].children) return false

      if (this.categorySelected === this.menu[index])
        this.categorySelected = null
      else this.categorySelected = this.menu[index]
    },
    closeDropdown() {
      this.categorySelected = null
    }
  }
}
</script>

<style scoped>
.menu {
  display: flex;
  padding: 0 50px;
  /*position: relative;*/
}
.menu-mobile {
  background: #f14b13
    url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjciIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNyAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48bGluZSB4MT0iMS41IiB5MT0iMS41IiB4Mj0iMjUuNSIgeTI9IjEuNSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIzIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiLz48bGluZSB4MT0iMS41IiB5MT0iMTIuNSIgeDI9IjI1LjUiIHkyPSIxMi41IiBzdHJva2U9IndoaXRlIiBzdHJva2Utd2lkdGg9IjMiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIvPjxsaW5lIHgxPSIxLjUiIHkxPSIyMi41IiB4Mj0iMjUuNSIgeTI9IjIyLjUiIHN0cm9rZT0id2hpdGUiIHN0cm9rZS13aWR0aD0iMyIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIi8+PC9zdmc+')
    no-repeat center;
  width: 46px;
  height: 38px;
  cursor: pointer;
  border-radius: 2px;
}
.menu-mobile:hover {
  background-color: #ef3b00;
}
.item {
  display: flex;
  align-items: center;
  cursor: pointer;
  position: relative;
  padding: 22px 25px;
}

.item:hover,
.item--selected {
  background: #ef3b00;
}
.item__label {
  white-space: nowrap;
}
.item__arrow {
  background: url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iOCIgaGVpZ2h0PSI1IiB2aWV3Qm94PSIwIDAgOCA1IiBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxwYXRoIGQ9Ik03LjgxMDE0IDAuNTcwMzU1TDcuNDI1MTMgMC4xODgzNDhDNy4yOTE2IDAuMDYyODg2NyA3LjEzNTg1IDAgNi45NTc5NiAwQzYuNzc2NDUgMCA2LjYyMjI3IDAuMDYyODg2NyA2LjQ5NTc1IDAuMTg4MzQ4TDMuOTk5OTYgMi42NjMxMUwxLjUwNDU2IDAuMTg4MzQ4QzEuMzc3NzMgMC4wNjI4ODY3IDEuMjIzODcgMCAxLjA0MjI4IDBDMC44NjQ0NjcgMCAwLjcwODcxNiAwLjA2Mjg4NjcgMC41NzUxODIgMC4xODgzNDhMMC4xOTUxNDEgMC41NzAzNTVDMC4wNjQ5MTU4IDAuNjk5NDg4IDAgMC44NTM4NTMgMCAxLjAzMzYxQzAgMS4yMTcwMyAwLjA2NTIzMDkgMS4zNjk5MSAwLjE5NTE0MSAxLjQ5MTk0TDMuNTM3NzUgNC44MDY1N0MzLjY2MTIgNC45MzU2MyAzLjgxNTA2IDUgMy45OTk5NiA1QzQuMTgxNTUgNSA0LjMzNzMgNC45MzU2MyA0LjQ2NzEzIDQuODA2NTdMNy44MTAxNCAxLjQ5MTk0QzcuOTM2NTggMS4zNjYyNCA4IDEuMjEzNjcgOCAxLjAzMzYxQzggMC44NTcyMTIgNy45MzY1OCAwLjcwMjc2OSA3LjgxMDE0IDAuNTcwMzU1WiIgZmlsbD0id2hpdGUiLz48L3N2Zz4=')
    no-repeat center;
  width: 8px;
  height: 5px;
  margin-left: 20px;
  transition: transform 0.3s;
}
.item--selected .item__arrow {
  transform: rotate(180deg);
}
.dropdown {
  max-width: 1440px;
  margin: auto;
  height: 400px;
  left: 0;
  right: 0;
  position: absolute;
  top: 65px;
}
.dropdown__overlay {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  top: 68px;
  margin: auto;
  background: rgba(0, 0, 0, 0.8);
  cursor: pointer;
}
.dropdown__wrapper {
  display: flex;
  background: #f3f7fa;
  box-shadow: inset 6px 10px 13px rgba(255, 92, 0, 0.28);
  position: relative;
  height: 100%;
}
.dropdown__children {
  padding: 40px 70px;
  background: rgba(255, 255, 255, 0.96);
  color: #ef3b00;
  width: 296px;
  height: 100%;
  font-size: 18px;
  font-weight: 500;
}
.dropdown__child {
  margin-bottom: 10px;
  cursor: pointer;
}
.dropdown__posts {
  flex: 1;
  padding: 40px;
  display: flex;
  overflow-x: scroll;
  overflow-y: hidden;
  margin-bottom: 35px;
}

.dropdown__posts::-webkit-scrollbar {
  height: 5px;
}

.dropdown__posts::-webkit-scrollbar-track {
  background: rgba(186, 192, 200, 0.34);
  border-radius: 10px;
}

.dropdown__posts::-webkit-scrollbar-thumb {
  background: #f25822;
  border-radius: 10px;
}

.dropdown__posts::-webkit-scrollbar-button {
  width: 20px;
}

.post {
  width: 306.83px;
  min-width: 306.83px;
  place-self: flex-start;
  margin-right: 20px;
  cursor: pointer;
  box-shadow: 0 4px 8px rgba(114, 162, 186, 0.09);
}
.post__thumbnail {
  display: block;
}
.post__footer {
  padding: 10px 25px;
  background: rgba(255, 255, 255, 0.45);
  transition: background-color 0.3s;
}
.post:hover .post__footer {
  background: #f25822;
}
.post__title {
  color: #303030;
  font-weight: 900;
}
.post__description {
  color: #aaaeb3;
}
.post__title,
.post__description {
  transition: color 0.3s;
}
.post:hover .post__title,
.post:hover .post__description {
  color: #ffffff;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.3s;
}

.fade-enter,
.fade-leave-to {
  opacity: 0;
}

.fade-enter-to,
.fade-leave {
  opacity: 1;
}

@media (max-width: 1200px) {
  .menu {
    padding: 0 25px;
  }
}

@media (max-width: 1120px) {
  .item {
    padding: 22px 15px;
  }
  .item__arrow {
    margin-left: 10px;
  }
}
</style>
