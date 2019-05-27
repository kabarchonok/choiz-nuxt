<template>
  <div class="feed">
    <div class="post">
      <div class="post__header">
        <div class="post__category">
          People <span class="post__category-slash">/</span> Celebrities
        </div>
        <div class="post__source">
          <img
            src="~/static/feed-source.png"
            alt=""
            class="post__source-icon"
          />mashable.com
        </div>
        <div class="post__repost">792</div>
      </div>
      <div class="post__title">
        Women-only «Wonder Woman» screenings were almost stupidly nice
      </div>
      <img src="~/static/feed-thumbnail.png" class="post__thumbnail" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'Feed'
}
</script>

<style scoped>
.feed {
  padding: 70px 40px 70px 70px;
  overflow-y: scroll;
  height: 100%;
  margin-right: 30px;
}

.post__header {
  display: flex;
  color: #c3c7cb;
  font-weight: 900;
  font-size: 14px;
  justify-content: flex-end;
  margin-bottom: 25px;
}
.post__category {
  color: #f25822;
  flex: 1;
  justify-self: flex-start;
}
.post__category-slash {
  color: #c3c7cb;
}
.post__source {
  display: flex;
  align-items: center;
  line-height: 16px;
  margin-right: 30px;
}
.post__source-icon {
  margin-right: 7px;
}
.post__repost {
  background: url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTciIGhlaWdodD0iMTYiIHZpZXdCb3g9IjAgMCAxNyAxNiIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNMTYuODE5OSA1LjMxMDAxTDExLjk2MjcgMC4xOTAwNDhDMTEuODQyNSAwLjA2MzM2MTEgMTEuNzAwMiAzLjMxMzU3ZS0wOCAxMS41MzU4IDMuMzEzNTdlLTA4QzExLjM3MTQgMy4zMTM1N2UtMDggMTEuMjI5IDAuMDYzMzYxMSAxMS4xMDg5IDAuMTkwMDQ4QzEwLjk4ODcgMC4zMTY4MDYgMTAuOTI4NiAwLjQ2NjgyIDEwLjkyODYgMC42NDAxMjZWMy4yMDAxMUg4LjgwMzU4QzQuMjk0MSAzLjIwMDExIDEuNTI3MzMgNC41NDM0NyAwLjUwMjYzIDcuMjMwMTRDMC4xNjc1MzIgOC4xMjMzNiAwIDkuMjMzNDkgMCAxMC41NjAyQzAgMTEuNjY2OCAwLjQwMTYxOSAxMy4xNyAxLjIwNDc5IDE1LjA3MDFDMS4yMjM3MyAxNS4xMTY5IDEuMjU2ODIgMTUuMTk2NyAxLjMwNDM0IDE1LjMxQzEuMzUxODIgMTUuNDIzMiAxLjM5NDQ1IDE1LjUyMzIgMS40MzI0IDE1LjYxQzEuNDcwNDggMTUuNjk2NSAxLjUxMTYxIDE1Ljc2OTkgMS41NTU4NCAxNS44Mjk4QzEuNjMxNjYgMTUuOTQzMiAxLjcyMDI1IDE2IDEuODIxNDYgMTZDMS45MTYzMiAxNiAxLjk5MDY1IDE1Ljk2NjcgMi4wNDQ0NCAxNS45QzIuMDk4MTEgMTUuODMzNCAyLjEyNDk5IDE1Ljc1IDIuMTI0OTkgMTUuNjUwMkMyLjEyNDk5IDE1LjU5MDEgMi4xMTcwOCAxNS41MDE5IDIuMTAxMjMgMTUuMzg1MUMyLjA4NTQxIDE1LjI2ODQgMi4wNzc0NyAxNS4xOTAyIDIuMDc3NDcgMTUuMTUwMkMyLjA0NTgxIDE0LjY5NyAyLjAyOTk5IDE0LjI4NjcgMi4wMjk5OSAxMy45MjAzQzIuMDI5OTkgMTMuMjQ3IDIuMDg1NDEgMTIuNjQzNiAyLjE5NTk5IDEyLjExMDNDMi4zMDY3NCAxMS41NzY5IDIuNDYwMDkgMTEuMTE1NCAyLjY1NjE5IDEwLjcyNTNDMi44NTIyNyAxMC4zMzUxIDMuMTA1MTYgOS45OTg3MyAzLjQxNTE0IDkuNzE1MzdDMy43MjQ5OCA5LjQzMjAyIDQuMDU4NTUgOS4yMDA0MyA0LjQxNTg4IDkuMDIwNEM0Ljc3MzI3IDguODQwMzMgNS4xOTM4MyA4LjY5ODY1IDUuNjc3NjUgOC41OTUzNkM2LjE2MTQ0IDguNDkyMDQgNi42NDgzOSA4LjQyMDM0IDcuMTM4NTkgOC4zODAzMUM3LjYyODggOC4zNDAyNyA4LjE4Mzc2IDguMzIwMzggOC44MDM1OCA4LjMyMDM4SDEwLjkyODZWMTAuODgwNEMxMC45Mjg2IDExLjA1MzcgMTAuOTg4NiAxMS4yMDM4IDExLjEwODcgMTEuMzMwNEMxMS4yMjkgMTEuNDU2OSAxMS4zNzEyIDExLjUyMDQgMTEuNTM1NiAxMS41MjA0QzExLjcgMTEuNTIwNCAxMS44NDIzIDExLjQ1NjkgMTEuOTYyNyAxMS4zMzA0TDE2LjgxOTggNi4yMTAyN0MxNi45NCA2LjA4MzU4IDE3IDUuOTMzNjQgMTcgNS43NjAyOUMxNyA1LjU4Njk5IDE2Ljk0IDUuNDM2OTQgMTYuODE5OSA1LjMxMDAxWiIgZmlsbD0iI0VGM0IwMCIvPjwvc3ZnPg==')
    no-repeat left;
  padding-left: 26px;
}
.post__title {
  font-family: 'Rokkitt', serif;
  font-weight: 800;
  font-size: 36px;
  line-height: 37px;
  color: #303030;
  margin-bottom: 40px;
}
.post__thumbnail {
  display: block;
  width: 100%;
}
@media (min-width: 1000px) {
  .feed::-webkit-scrollbar {
    width: 3px;
  }

  .feed::-webkit-scrollbar-track {
    background: transparent;
    border-radius: 10px;
  }

  .feed:hover::-webkit-scrollbar-track {
    background: rgba(186, 192, 200, 0.34);
    border-radius: 10px;
  }

  .feed::-webkit-scrollbar-thumb {
    background: transparent;
    border-radius: 10px;
    opacity: 0;
  }

  .feed:hover::-webkit-scrollbar-thumb {
    background: #f25822;
  }

  .feed::-webkit-scrollbar-button {
    height: 70px;
  }
}
@media (max-width: 999px) {
  .feed {
    padding: 70px 20px 70px 20px;
    margin-right: 0;
    overflow: auto;
  }
}
</style>
