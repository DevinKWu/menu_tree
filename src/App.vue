<template>
  <div id="app">
    <Menu :menuList="menuList"></Menu>
  </div>
</template>

<script>
import Menu from "./components/Menu";
// let MenuItem = require("./components/MenuItem");

export default {
  components: {
    Menu
  },
  data() {
    return {
      menuList: [
        {
          label: "24h購物(2065)",
          children: [
            {
              label: "電玩/遊戲(522)",
              children: [
                {
                  label: "►PS4 遊戲(127)",
                  children: [
                    {
                      label: "電玩/遊戲(522)",
                      children: [
                        {
                          label: "►PS4 遊戲(127)"
                        },
                        {
                          label: "►Switch 遊戲(63)"
                        }
                      ]
                    },
                    {
                      label: "積木桌遊(495)",
                      children: [
                        {
                          label: "◆ 德國HABA桌遊(88)"
                        },
                        {
                          label: "■趣味桌遊/ 玩具(81)"
                        }
                      ]
                    }
                  ]
                },
                {
                  label: "►Switch 遊戲(63)"
                }
              ]
            },
            {
              label: "積木桌遊(495)",
              children: [
                {
                  label: "◆ 德國HABA桌遊(88)"
                },
                {
                  label: "■趣味桌遊/ 玩具(81)"
                }
              ]
            }
          ]
        },
        {
          label: "24h購物(2065)",
          children: [
            {
              label: "電玩/遊戲(522)",
              children: [
                {
                  label: "►PS4 遊戲(127)",
                  children: [
                    {
                      label: "電玩/遊戲(522)",
                      children: [
                        {
                          label: "►PS4 遊戲(127)"
                        },
                        {
                          label: "►Switch 遊戲(63)"
                        }
                      ]
                    },
                    {
                      label: "積木桌遊(495)",
                      children: [
                        {
                          label: "◆ 德國HABA桌遊(88)"
                        },
                        {
                          label: "■趣味桌遊/ 玩具(81)"
                        }
                      ]
                    }
                  ]
                },
                {
                  label: "►Switch 遊戲(63)"
                }
              ]
            },
            {
              label: "積木桌遊(495)",
              children: [
                {
                  label: "◆ 德國HABA桌遊(88)"
                },
                {
                  label: "■趣味桌遊/ 玩具(81)"
                }
              ]
            }
          ]
        }
      ]
    };
  }
};
</script>

<style>
ul {
  list-style: none;
  line-height: 20px;
}

.item > span {
  display: inline-block;
  width: 20px;
  height: 20px;
  text-align: center;
  background-color: #eee;
  border: 1px solid;
  box-sizing: border-box;
}
</style>
