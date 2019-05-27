<template>
  <div class="lang">
    <div class="lang__arrow"></div>
    En
  </div>
</template>

<script>
export default {
  name: 'HeaderDropdownLanguage'
}
</script>

<style scoped>
.lang {
  font-size: 16px;
  line-height: 18px;
  font-weight: bold;
  background: #f14b13;
  padding: 10px;
  border-radius: 2px;
  height: 38px;
  width: 58px;
  min-width: 58px;
  position: relative;
  cursor: pointer;
  transition: background-color 0.3s;
}
.lang:hover {
  background: #ef3b00;
}
.lang__arrow {
  background: url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iOCIgaGVpZ2h0PSI1IiB2aWV3Qm94PSIwIDAgOCA1IiBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxwYXRoIGQ9Ik03LjgxMDE0IDAuNTcwMzU1TDcuNDI1MTMgMC4xODgzNDhDNy4yOTE2IDAuMDYyODg2NyA3LjEzNTg1IDAgNi45NTc5NiAwQzYuNzc2NDUgMCA2LjYyMjI3IDAuMDYyODg2NyA2LjQ5NTc1IDAuMTg4MzQ4TDMuOTk5OTYgMi42NjMxMUwxLjUwNDU2IDAuMTg4MzQ4QzEuMzc3NzMgMC4wNjI4ODY3IDEuMjIzODcgMCAxLjA0MjI4IDBDMC44NjQ0NjcgMCAwLjcwODcxNiAwLjA2Mjg4NjcgMC41NzUxODIgMC4xODgzNDhMMC4xOTUxNDEgMC41NzAzNTVDMC4wNjQ5MTU4IDAuNjk5NDg4IDAgMC44NTM4NTMgMCAxLjAzMzYxQzAgMS4yMTcwMyAwLjA2NTIzMDkgMS4zNjk5MSAwLjE5NTE0MSAxLjQ5MTk0TDMuNTM3NzUgNC44MDY1N0MzLjY2MTIgNC45MzU2MyAzLjgxNTA2IDUgMy45OTk5NiA1QzQuMTgxNTUgNSA0LjMzNzMgNC45MzU2MyA0LjQ2NzEzIDQuODA2NTdMNy44MTAxNCAxLjQ5MTk0QzcuOTM2NTggMS4zNjYyNCA4IDEuMjEzNjcgOCAxLjAzMzYxQzggMC44NTcyMTIgNy45MzY1OCAwLjcwMjc2OSA3LjgxMDE0IDAuNTcwMzU1WiIgZmlsbD0id2hpdGUiLz48L3N2Zz4=')
    no-repeat center;
  width: 8px;
  height: 5px;
  position: absolute;
  right: 10px;
  top: 0;
  bottom: 0;
  margin: auto;
}
</style>
