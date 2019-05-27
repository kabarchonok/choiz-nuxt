<template>
  <header class="header">
    <div class="header__wrapper">
      <Logo></Logo>
      <HeaderDropdownLanguage></HeaderDropdownLanguage>
      <HeaderNavigationMenu></HeaderNavigationMenu>
      <div class="search"></div>
      <div class="account"></div>
    </div>
  </header>
</template>

<script>
import Logo from './Logo'
import HeaderDropdownLanguage from './HeaderDropdownLanguage'
import HeaderNavigationMenu from './HeaderNavigationMenu'

export default {
  name: 'Header',
  components: {
    Logo,
    HeaderDropdownLanguage,
    HeaderNavigationMenu
  }
}
</script>

<style scoped>
.header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  background: #f25822;
  border-top: 3px solid #ef3b00;
  box-shadow: 0 10px 13px rgba(255, 92, 0, 0.28);
  color: #ffffff;
  z-index: 10000;
}
.header__wrapper {
  padding-left: 70px;
  max-width: 1440px;
  margin: auto;
  display: flex;
  align-items: center;
}
.search {
  background: #f14b13
    url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTgiIGhlaWdodD0iMTgiIHZpZXdCb3g9IjAgMCAxOCAxOCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNNy4xODc5MSAxMy41MzYxQzguNzM1MjMgMTMuNTM2MSAxMC4xNDE3IDEyLjk4NzQgMTEuMjM5MSAxMi4wNTk2TDE2LjE2MTkgMTYuOTgyNEMxNi4yNzQ2IDE3LjA5NDIgMTYuNDE0NyAxNy4xNTA3IDE2LjU2OTggMTcuMTUwN0MxNi43MjQzIDE3LjE1MDcgMTYuODY1MSAxNy4wOTQyIDE2Ljk3NzggMTYuOTgyNEMxNy4yMDIzIDE2Ljc1NyAxNy4yMDIzIDE2LjM5MSAxNi45Nzc4IDE2LjE2NjVMMTIuMDU1MSAxMS4yNDM3QzEyLjk2OTEgMTAuMTQ2MyAxMy41MzE2IDguNzI2MDQgMTMuNTMxNiA3LjE5MjQyQzEzLjUzMTYgMy42OTA1NyAxMC42OTA0IDAuODQ5NDI2IDcuMTg3OTEgMC44NDk0MjZDMy42OTk4IDAuODQ5NDI2IDAuODQ0OTcxIDMuNzA0MjggMC44NDQ5NzEgNy4xOTI0MkMwLjg0NDk3MSAxMC42OTUgMy42OTk4IDEzLjUzNjEgNy4xODc5MSAxMy41MzYxWk03LjE4NzkxIDIuMDAyNTlDMTAuMDU3MiAyLjAwMjU5IDEyLjM3ODYgNC4zMzc1NiAxMi4zNzg2IDcuMTkyNDJDMTIuMzc4NiAxMC4wNjE3IDEwLjA1NzIgMTIuMzgzMSA3LjE4NzkxIDEyLjM4MzFDNC4zMTkzNiAxMi4zODMxIDEuOTk4MTIgMTAuMDQ4IDEuOTk4MTIgNy4xOTI0MkMxLjk5ODEyIDQuMzM3NTYgNC4zMzMwOCAyLjAwMjU5IDcuMTg3OTEgMi4wMDI1OVoiIGZpbGw9IndoaXRlIi8+PC9zdmc+')
    no-repeat center;
  width: 45px;
  min-width: 45px;
  height: 38px;
  margin-right: 25px;
  cursor: pointer;
}
.search:hover {
  background-color: #ef3b00;
}
.account {
  background: #f14b13
    url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTciIGhlaWdodD0iMTgiIHZpZXdCb3g9IjAgMCAxNyAxOCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNNi41Njk0MiAxMi4xMDgzQzMuODg4ODggMTIuNDQ2OCAxLjMxNjkgMTIuODcyNCAtNS41OTE4MWUtMDggMTUuNjExNUMyLjczNzU5IDE3LjYyMzQgNS4xMTYyNCAxNy45ODA1IDguMzQxMTMgMTcuOTk5OEMxMS4xMDQxIDE4LjAwNDcgMTUuMTU0NiAxNy45MjQxIDE3IDE1LjU2MzFDMTUuODY2MSAxMy41NjgxIDEzLjAxODQgMTIuMTA1OSAxMC4zNzk5IDEyLjA4MjVMMTAuMzUxMyAxMC40NjcxQzEyLjQ3MDEgOC41MTMyNCAxMy4yNTY5IDQuMTc4MjEgMTEuOTIwMiAxLjg0MjIzQzExLjA4MTkgMC40NTk4MjggOS44ODA2OCAwLjAxODEwMzkgOC4yOTc1NSAwLjAwMDM3MDQzMUM2LjY4MjczIC0wLjAxODE2OTEgNS45Mzk1IDAuNjU5NzMzIDQuOTcxMjQgMS44OTMwMUMzLjMyNDczIDQuNjQ4OTUgNC42MDkxNCA4Ljc5MTMzIDYuNTY5NDIgMTAuNDc2IiBmaWxsPSJ3aGl0ZSIvPjwvc3ZnPg==')
    no-repeat center;
  width: 38px;
  min-width: 38px;
  height: 38px;
  margin-right: 25px;
  border-radius: 50%;
  cursor: pointer;
}
.account:hover {
  background-color: #ef3b00;
}
@media (max-width: 1200px) {
  .header__wrapper {
    justify-content: space-between;
  }
}
@media (max-width: 999px) {
  .header {
    padding: 0 20px;
  }
  .header__wrapper {
    padding: 0;
  }
  .account {
    margin-right: 0;
  }
}
</style>
