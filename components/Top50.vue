<template>
  <div v-if="width >= 999" class="top50">
    <div class="top50__pin"></div>
    <div class="top50__inner">
      <div class="icon"></div>
      <div class="title">Top 50</div>
      <div class="description">topics, that are discussed today</div>
      <div class="posts">
        <div class="post">
          <div class="post__position">1</div>
          <div class="post__inner">
            <img
              src="~/static/top50-thumbnail.png"
              alt=""
              class="post__thumbnail"
            />
            <div class="post__footer">
              <div class="post__title">
                Dude Discovers His Talent On Fidget Spinne
              </div>
            </div>
          </div>
          <div class="post__actions">
            <div class="repost">149 284</div>
          </div>
        </div>
        <div class="post">
          <div class="post__position">2</div>
          <div class="post__inner">
            <img
              src="~/static/top50-thumbnail.png"
              alt=""
              class="post__thumbnail"
            />
            <div class="post__footer">
              <div class="post__title">
                Dude Discovers His Talent On Fidget Spinne
              </div>
            </div>
          </div>
          <div class="post__actions">
            <div class="repost">149 284</div>
          </div>
        </div>
        <div class="post">
          <div class="post__position">3</div>
          <div class="post__inner">
            <img
              src="~/static/top50-thumbnail.png"
              alt=""
              class="post__thumbnail"
            />
            <div class="post__footer">
              <div class="post__title">
                Dude Discovers His Talent On Fidget Spinne
              </div>
            </div>
          </div>
          <div class="post__actions">
            <div class="repost">149 284</div>
          </div>
        </div>
        <div class="post">
          <div class="post__position">4</div>
          <div class="post__inner">
            <img
              src="~/static/top50-thumbnail.png"
              alt=""
              class="post__thumbnail"
            />
            <div class="post__footer">
              <div class="post__title">
                Dude Discovers His Talent On Fidget Spinne
              </div>
            </div>
          </div>
          <div class="post__actions">
            <div class="repost">149 284</div>
          </div>
        </div>
        <div class="post">
          <div class="post__position">5</div>
          <div class="post__inner">
            <img
              src="~/static/top50-thumbnail.png"
              alt=""
              class="post__thumbnail"
            />
            <div class="post__footer">
              <div class="post__title">
                Dude Discovers His Talent On Fidget Spinne
              </div>
            </div>
          </div>
          <div class="post__actions">
            <div class="repost">149 284</div>
          </div>
        </div>
        <div class="post">
          <div class="post__position">6</div>
          <div class="post__inner">
            <img
              src="~/static/top50-thumbnail.png"
              alt=""
              class="post__thumbnail"
            />
            <div class="post__footer">
              <div class="post__title">
                Dude Discovers His Talent On Fidget Spinne
              </div>
            </div>
          </div>
          <div class="post__actions">
            <div class="repost">149 284</div>
          </div>
        </div>
        <div class="post">
          <div class="post__position">7</div>
          <div class="post__inner">
            <img
              src="~/static/top50-thumbnail.png"
              alt=""
              class="post__thumbnail"
            />
            <div class="post__footer">
              <div class="post__title">
                Dude Discovers His Talent On Fidget Spinne
              </div>
            </div>
          </div>
          <div class="post__actions">
            <div class="repost">149 284</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Top50',
  data() {
    return {
      width: 0
    }
  },
  mounted() {
    window.addEventListener('resize', this.updateWidth)
    this.updateWidth()
  },
  methods: {
    updateWidth() {
      this.width = window.innerWidth
    }
  }
}
</script>

<style scoped>
.top50 {
  width: 296px;
  height: 100%;
  position: relative;
  background: #fffcf7;
}
.top50__pin {
  background: url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNMTcuMzc2NSAxNy4zNDU1QzE3LjM3NjcgMTYuMTg0OCAxNi43NzU1IDE0Ljk5NTIgMTUuNTg5NCAxMy44MDkxQzE1LjMzODMgMTMuNTU4IDE1LjA1OTcgMTMuMzA2NSAxNC43NTk1IDEzLjA1OTVMMTQuNjAzMyA3LjUwMzczTDE1Ljk2NzQgNy41MDM3QzE2LjIyMDMgNy41MDM1OSAxNi40MjUzIDcuMjk4NiAxNi40MjU0IDcuMDQ1NDhMMTYuNDI1OCA1LjE1MjI3QzE2LjQyNTkgNC45MDkzMyAxNi4yMTA4IDQuNjk0MjcgMTUuOTY3OSA0LjY5NDM0TDcuNDkzNzcgNC42OTU5N0M3LjI0MDc3IDQuNjk2MDEgNy4wMzU3NyA0LjkwMSA3LjAzNTY2IDUuMTUzOTRMNy4wMzUzNyA3LjA0NjcyQzcuMDM1NDIgNy4xNjgyNCA3LjA4MzU5IDcuMjg0NyA3LjE2OTUyIDcuMzcwNjRDNy4yNTUzOSA3LjQ1NjUgNy4zNzE5MiA3LjUwNDc0IDcuNDkzMzcgNy41MDQ3Mkw4Ljg1NzU0IDcuNTA0NzZMOC42OTk3NiAxMy4wNjA1QzcuNDY3MTcgMTQuMDc0NyA2LjA4MTM1IDE1LjYwMzEgNi4wODExMiAxNy4zNDcyQzYuMDgxMSAxNy40NzM3IDYuMTMyMzUgMTcuNTg4MiA2LjIxNTE3IDE3LjY3MUM2LjI5ODA2IDE3Ljc1MzkgNi40MTI2NiAxNy44MDUyIDYuNTM5MTIgMTcuODA1MkwxMS4yNzA5IDE3LjgwNDNMMTEuMjcwMiAyMS40Mjg1QzExLjI3MDMgMjEuNTU1MSAxMS4zMjE1IDIxLjY2OTUgMTEuNDA0NCAyMS43NTI0QzExLjQ4NzIgMjEuODM1MiAxMS42MDE5IDIxLjg4NjUgMTEuNzI4MyAyMS44ODY1QzExLjk4MTMgMjEuODg2NSAxMi4xODY0IDIxLjY4MTQgMTIuMTg2NCAyMS40Mjg0TDEyLjE4NjkgMTcuODA0MkwxNi45MTg0IDE3LjgwMzdDMTcuMTcxNCAxNy44MDM1IDE3LjM3NjMgMTcuNTk4NiAxNy4zNzY1IDE3LjM0NTVaTTcuMDM5OTcgMTYuODg4OEM3LjI3NTEyIDE1LjYwNjYgOC40NDEyNyAxNC40MzQzIDkuNDM2NjkgMTMuNjQyNEM5LjU0MjMyIDEzLjU1ODMgOS42MDU2OCAxMy40MzE4IDkuNjA5MzIgMTMuMjk2OUw5Ljc4NjggNy4wNTkzN0M5Ljc5MDI5IDYuOTM1NjYgOS43NDM0NSA2LjgxNjAxIDkuNjU3MjYgNi43MjczMUM5LjY1NTc2IDYuNzI1ODEgOS42NTQxOCA2LjcyNDIzIDkuNjUyNjggNi43MjI3M0M5LjU2NjgyIDYuNjM2ODcgOS40NTAyOCA2LjU4ODYzIDkuMzI4ODcgNi41ODg2MUw3Ljk1MTQ4IDYuNTg4NjhMNy45NTE2IDUuNjExOTRMMTUuNTA5NyA1LjYxMDQ5TDE1LjUwOTQgNi41ODc3M0wxNC4xMzIxIDYuNTg3ODNDMTQuMDA4MyA2LjU4Nzk5IDEzLjg5IDYuNjM3OTUgMTMuODAzNiA2LjcyNjg1QzEzLjcxNzUgNi44MTUzOSAxMy42NzA2IDYuOTM1NTYgMTMuNjc0MSA3LjA1OTE2TDEzLjg0OTYgMTMuMjk2MUMxMy44NTMyIDEzLjQzMTIgMTMuOTE2IDEzLjU1NzQgMTQuMDIyMiAxMy42NDE1QzE0LjM1OTYgMTMuOTA5OCAxNC42Njg5IDE0LjE4NDIgMTQuOTQxNSAxNC40NTY5QzE1Ljc4MiAxNS4yOTc0IDE2LjI3NzEgMTYuMTEyNyAxNi40MTgxIDE2Ljg4NzZMNy4wMzk5NyAxNi44ODg4WiIgZmlsbD0iI0YyNTgyMiIvPjwvc3ZnPg==')
    no-repeat center;
  width: 16.2px;
  height: 16.2px;
  position: absolute;
  top: 77px;
  right: 14px;
}
.top50__inner {
  height: 100%;
  padding: 70px 50px 70px 20px;
  margin-right: 20px;
  overflow-y: scroll;
}
.top50__inner::-webkit-scrollbar {
  width: 2px;
}

.top50__inner::-webkit-scrollbar-track {
  background: rgba(186, 192, 200, 0.34);
  border-radius: 10px;
}

.top50__inner::-webkit-scrollbar-thumb {
  background: #f25822;
  border-radius: 10px;
}

.top50__inner::-webkit-scrollbar-button {
  height: 130px;
}

.icon {
  width: 24.64px;
  height: 31px;
  background: url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjUiIGhlaWdodD0iMzEiIHZpZXdCb3g9IjAgMCAyNSAzMSIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNNi45MzY3MiAzMUM1LjA0NTI3IDI2LjcwMSA2LjA1MjU0IDI0LjIzNzYgNy41MDYyNSAyMS45MTY3QzkuMDk4MjIgMTkuMzc1IDkuNTA4NDggMTYuODU5MSA5LjUwODQ4IDE2Ljg1OTFDOS41MDg0OCAxNi44NTkxIDEwLjc1OTkgMTguNjM2MSAxMC4yNTkzIDIxLjQxNTVDMTIuNDcwMiAxOC43MjcyIDEyLjg4NzQgMTQuNDQ0MSAxMi41NTM2IDEyLjgwMzdDMTcuNTUxIDE2LjYxODUgMTkuNjg2OCAyNC44Nzg0IDE2LjgwODUgMzFDMzIuMTE3NSAyMS41Mzg2IDIwLjYxNjUgNy4zODE1MyAxOC42MTQyIDUuNzg2ODFDMTkuMjgxNiA3LjM4MTQ3IDE5LjQwODIgMTAuMDgxMSAxOC4wNTk5IDExLjM5MTJDMTUuNzc3NSAxLjkzNzQ4IDEwLjEzNDIgMCAxMC4xMzQyIDBDMTAuODAxNyA0Ljg3NTM1IDcuNzE0ODUgMTAuMjA2NSA0LjczODI0IDE0LjE5MDFDNC42MzM2NyAxMi4yNDYgNC41MjI1NiAxMC45MDQ1IDMuNTg2NjYgOS4wNDQyQzMuMzc2NTggMTIuNTc1OCAwLjkwNTc1MyAxNS40NTQ1IDAuMjM2NjU3IDE4Ljk5MjlDLTAuNjY5NjYyIDIzLjc4NDggMC45MTU1NDMgMjcuMjkzMyA2LjkzNjcyIDMxWiIgZmlsbD0iI0VGM0IwMCIvPjwvc3ZnPg==')
    no-repeat center;
  margin-bottom: 23px;
}
.title {
  color: #303030;
  font-family: 'Rokkitt', serif;
  font-style: normal;
  font-weight: 800;
  font-size: 36px;
}
.description {
  color: #a9adb2;
  font-size: 12px;
  font-weight: 800;
  margin-bottom: 40px;
}

.post {
  width: 197px;
  position: relative;
  margin-bottom: 20px;
}
.post__position {
  position: absolute;
  font-family: 'Rokkitt', serif;
  font-style: normal;
  font-weight: 900;
  font-size: 24px;
  line-height: 30px;
  z-index: 1;
  background: #fffcf7;
  border-radius: 50%;
  width: 30px;
  height: 30px;
  text-align: center;
  color: #ef3b00;
  left: -15px;
  top: -15px;
}
.post__inner {
  min-height: 197px;
  border-radius: 4px;
  position: relative;
  cursor: pointer;
}
.post__thumbnail {
  display: block;
  width: 100%;
  position: absolute;
  filter: grayscale(100%);
  transition: filter 0.3s;
}
.post__footer {
  position: absolute;
  bottom: 0;
  background: rgba(255, 252, 247, 0.89);
  padding: 10px 15px;
  font-size: 14px;
  font-weight: bold;
  color: #303030;
}
.post__actions {
  padding: 10px 0;
  display: flex;
  justify-content: flex-end;
  color: #ef3b00;
}
.repost {
  background: url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTkiIGhlaWdodD0iMTgiIHZpZXdCb3g9IjAgMCAxOSAxOCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNMTcuOTA2IDUuNjczMDdDMTcuOTA1MyA1LjY3MjM5IDE3LjkwNDcgNS42NzE3MiAxNy45MDQxIDUuNjcxMDRMMTIuNzM0NSAwLjIwMzAxNEMxMi43MzQ1IDAuMjAzMDA5IDEyLjczNDUgMC4yMDMwMDQgMTIuNzM0NCAwLjIwMjk5OUMxMi42MDY1IDAuMDY3Njc4NyAxMi40NTUxIDMuNTM5NWUtMDggMTIuMjggMy41Mzk1ZS0wOEMxMi4xMDUgMy41Mzk1ZS0wOCAxMS45NTM1IDAuMDY3NjQ3NSAxMS44MjU3IDAuMjAyOTA1QzExLjgyNTcgMC4yMDI5NzIgMTEuODI1NiAwLjIwMzA0IDExLjgyNTUgMC4yMDMxMDdDMTEuNjk3NyAwLjMzODQ4NiAxMS42MzM2IDAuNDk4Njk0IDExLjYzMzYgMC42ODM3NzFWMS40MTgyOUMxMS42MzM2IDIuNTIyODYgMTAuNzM4MiAzLjQxODI5IDkuNjMzNjQgMy40MTgyOUg5LjM3MTU2QzQuNTc0IDMuNDE4MjkgMS42MjkzNyA0Ljg1MTU1IDAuNTM3MDA4IDcuNzE3OThDMC41MzU3MTUgNy43MjEzNyAwLjUzNDQyOSA3LjcyNDc4IDAuNTMzMTYgNy43MjgxOUMwLjE3NzcwOCA4LjY4MTQzIDAgOS44NjU1NyAwIDExLjI4MDJIMEMwIDEyLjQ1OTUgMC40MjU1NyAxNC4wNjA2IDEuMjc2NjQgMTYuMDgzN0MxLjI4MDUzIDE2LjA5MjkgMS4yODQzOCAxNi4xMDIzIDEuMjg4MTYgMTYuMTExNUMxLjMwODk2IDE2LjE2MjggMS4zNDIzMyAxNi4yNDM0IDEuMzg4NDggMTYuMzUzOEMxLjM4ODQ5IDE2LjM1MzkgMS4zODg0OSAxNi4zNTM5IDEuMzg4NSAxNi4zNTM5QzEuNDM4NjggMTYuNDc0IDEuNDgzNzcgMTYuNTgwMSAxLjUyMzk0IDE2LjY3MjNDMS41MjQ1MiAxNi42NzM3IDEuNTI1MSAxNi42NzUgMS41MjU2OSAxNi42NzYzQzEuNTU4MjggMTYuNzUwNCAxLjU5Mjk4IDE2LjgxNTQgMS42Mjk3OSAxNi44NzEyQzEuNjQ2NzcgMTYuODk2OSAxLjY2NDMgMTYuOTIyMyAxLjY4MzIgMTYuOTQ2N0MxLjc1NzczIDE3LjA0MjggMS44NDMwMiAxNy4wOTA5IDEuOTM4OTcgMTcuMDkwOUMyLjAzOTYgMTcuMDkwOSAyLjExODUzIDE3LjA1NTYgMi4xNzU3NCAxNi45ODQ5QzIuMTc2MTQgMTYuOTg0NCAyLjE3NjU0IDE2Ljk4MzkgMi4xNzY5NCAxNi45ODM0QzIuMjMzNjcgMTYuOTEyNCAyLjI2MjA4IDE2LjgyMzUgMi4yNjIwOCAxNi43MTczQzIuMjYyMDggMTYuNjUzMSAyLjI1MzY4IDE2LjU1OSAyLjIzNjgzIDE2LjQzNDRDMi4yMzY4MSAxNi40MzQyIDIuMjM2NzggMTYuNDM0IDIuMjM2NzYgMTYuNDMzOEMyLjIyNjU2IDE2LjM1ODMgMi4yMTk0NCAxNi4yOTc5IDIuMjE1NDIgMTYuMjUyNUMyLjIxMTMzIDE2LjIwNjQgMi4yMDk4NiAxNi4xNiAyLjIwNjc2IDE2LjExMzdDMi4xNzYyMiAxNS42NTcxIDIuMTYwOTYgMTUuMjQyIDIuMTYwOTYgMTQuODY5NEMyLjE2MDk2IDE0LjE1MDMgMi4yMTk5NCAxMy41MDU5IDIuMzM3NjIgMTIuOTM2M0MyLjMzNzY1IDEyLjkzNjEgMi4zMzc2OSAxMi45MzYgMi4zMzc3MiAxMi45MzU4QzIuNDU1NTkgMTIuMzY2MiAyLjYxODc4IDExLjg3MzMgMi44Mjc0NyAxMS40NTY4QzIuODI3NTMgMTEuNDU2NyAyLjgyNzU5IDExLjQ1NjUgMi44Mjc2NiAxMS40NTY0QzMuMDM2MzMgMTEuMDM5OCAzLjMwNTQ2IDEwLjY4MDUgMy42MzUzMSAxMC4zNzc5QzMuNjM1NDIgMTAuMzc3OCAzLjYzNTUyIDEwLjM3NzcgMy42MzU2MyAxMC4zNzc2QzMuOTY1NDIgMTAuMDc1IDQuMzIwNDUgOS44Mjc3IDQuNzAwNzcgOS42MzU0M0M0LjcwMDc3IDkuNjM1NDMgNC43MDA3OCA5LjYzNTQzIDQuNzAwNzggOS42MzU0MkM1LjA4MTIxIDkuNDQzMDkgNS41Mjg4NyA5LjI5MTc2IDYuMDQzODcgOS4xODE0M0M2LjA0MzkzIDkuMTgxNDIgNi4wNDM5OCA5LjE4MTQxIDYuMDQ0MDQgOS4xODEzOUM2LjU1OTAxIDkuMDcxMDMgNy4wNzczNSA4Ljk5NDQ1IDcuNTk5MTUgOC45NTE2OUM4LjEyMDk4IDguOTA4OTMgOC43MTE3NCA4Ljg4NzY4IDkuMzcxNTYgOC44ODc2OEg5LjYzMzY0QzEwLjczODIgOC44ODc2OCAxMS42MzM2IDkuNzgzMTEgMTEuNjMzNiAxMC44ODc3VjExLjYyMjNDMTEuNjMzNiAxMS44MDcgMTEuNjk3MyAxMS45NjcgMTEuODI0NiAxMi4xMDIxQzExLjgyNTEgMTIuMTAyNyAxMS44MjU2IDEyLjEwMzIgMTEuODI2MSAxMi4xMDM3QzExLjk1NCAxMi4yMzg0IDEyLjEwNTIgMTIuMzA1OSAxMi4yNzk4IDEyLjMwNTlDMTIuNDU0NCAxMi4zMDU5IDEyLjYwNTcgMTIuMjM4NCAxMi43MzM2IDEyLjEwMzhDMTIuNzM0MiAxMi4xMDMyIDEyLjczNDcgMTIuMTAyNiAxMi43MzUzIDEyLjEwMkwxNy45MDQ5IDYuNjMzNzFDMTcuOTA0OSA2LjYzMzcgMTcuOTA0OSA2LjYzMzY5IDE3LjkwNDkgNi42MzM2OEMxOC4wMzI4IDYuNDk4NDEgMTguMDk2NyA2LjMzODMxIDE4LjA5NjggNi4xNTMyM0MxOC4wOTY4IDYuMTUzMTEgMTguMDk2OCA2LjE1Mjk4IDE4LjA5NjggNi4xNTI4NUMxOC4wOTY3IDUuOTY4MjcgMTguMDMzMSA1LjgwODM5IDE3LjkwNiA1LjY3MzA3WiIgZmlsbD0iI0E3QUVCNCIvPjwvc3ZnPg==')
    no-repeat left;
  font-size: 14px;
  padding-left: 26px;
  font-weight: bold;
  cursor: pointer;
}
.post__inner:hover .post__thumbnail {
  filter: grayscale(0);
}
</style>
