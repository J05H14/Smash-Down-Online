<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <ul>
      <li><a href="https://vuejs.org" target="_blank">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank">Twitter</a></li>
    </ul>
    <h2>Ecosystem</h2>
    <ul>
      <li><a href="http://router.vuejs.org/" target="_blank">vue-router</a></li>
      <li><a href="http://vuex.vuejs.org/" target="_blank">vuex</a></li>
      <li><a href="http://vue-loader.vuejs.org/" target="_blank">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank">awesome-vue</a></li>
    </ul>
    <div v-for='char in characters' :src='char.img' :key='char.id'>
      {{char.name}}
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      test: 'test',
      characters: [
            {
              "name": "Mario",
              "id": "01",
              "img": "./assets/Char_Imgs/mario.png"
            },
            {
              "name": "Donkey Kong",
              "id": "02",
              "img": "./assets/Char_Imgs/donkey_kong.png"
            },
            {
              "name": "Link",
              "id": "03",
              "img": "./assets/Char_Imgs/link.png"
            },
            {
              "name": "Samus",
              "id": "04",
              "img": "./assets/Char_Imgs/samus.png"
            },
            {
              "name": "Dark Samus",
              "id": "05",
              "img": "./assets/Char_Imgs/dark_samus.png"
            },
            {
              "name": "Yoshi",
              "id": "06",
              "img": "./assets/Char_Imgs/yoshi.png"
            },
            {
              "name": "Kirby",
              "id": "07",
              "img": "./assets/Char_Imgs/kirby.png"
            },
            {
              "name": "Fox",
              "id": "08",
              "img": "./assets/Char_Imgs/fox.png"
            },
            {
              "name": "Pikachu",
              "id": "09",
              "img": "./assets/Char_Imgs/pikachu.png"
            },
            {
              "name": "Luigi",
              "id": "10",
              "img": "./assets/Char_Imgs/luigi.png"
            },
            {
              "name": "Ness",
              "id": "11",
              "img": "./assets/Char_Imgs/ness.png"
            },
            {
              "name": "Captain Falcon",
              "id": "12",
              "img": "./assets/Char_Imgs/captain_falcon.png"
            },
            {
              "name": "Jigglypuff",
              "id": "13",
              "img": "./assets/Char_Imgs/jigglypuff.png"
            },
            {
              "name": "Peach",
              "id": "14",
              "img": "./assets/Char_Imgs/peach.png"
            },
            {
              "name": "Daisy",
              "id": "15",
              "img": "./assets/Char_Imgs/daisy.png"
            },
            {
              "name": "Bowser",
              "id": "16",
              "img": "./assets/vvvvvChar_Imgs/bowser.png"
            },
            {
              "name": "Ice Climber",
              "id": "17",
              "img": "./assets/Char_Imgs/ice_climbers.png"
            },
            {
              "name": "Sheik",
              "id": "18",
              "img": "./assets/Char_Imgs/sheik.png"
            },
            {
              "name": "Zelda",
              "id": "19",
              "img": "./assets/Char_Imgs/zelda.png"
            },
            {
              "name": "Dr.Mario",
              "id": "20",
              "img": "./assets/Char_Imgs/dr_mario.png"
            },
            {
              "name": "Pichu",
              "id": "21",
              "img": "./assets/har_Imgs/pichu.png"
            },
            {
              "name": "Falco",
              "id": "22",
              "img": "./assets/Char_Imgs/falco.png"
            },
            {
              "name": "Marth",
              "id": "23",
              "img": "./assets/Char_Imgs/marth.png"
            },
            {
              "name": "Lucina",
              "id": "24",
              "img": "./assets/Char_Imgs/lucina.png"
            },
            {
              "name": "Young Link",
              "id": "25",
              "img": "./assets/Char_Imgs/young_link.png"
            },
            {
              "name": "Ganondorf",
              "id": "26",
              "img": "./assets/Char_Imgs/ganondorf.png"
            },
            {
              "name": "Mewtwo",
              "id": "27",
              "img": "./assets/Char_Imgs/mewtwo.png"
            },
            {
              "name": "Roy",
              "id": "28",
              "img": "./assets/Char_Imgs/roy.png"
            },
            {
              "name": "Chrom",
              "id": "29",
              "img": "./assets/Char_Imgs/chrom.png"
            },
            {
              "name": "Mr.Game & Watch",
              "id": "30",
              "img": "./assets/Char_Imgs/mr_game_and_watch.png"
            },
            {
              "name": "Meta Knight",
              "id": "31",
              "img": ""
            },
            {
              "name": "Pit",
              "id": "32",
              "img": ""
            },
            {
              "name": "Dark Pit",
              "id": "33",
              "img": ""
            },
            {
              "name": "Zero Suit Samus",
              "id": "34",
              "img": ""
            },
            {
              "name": "Wario",
              "id": "35",
              "img": ""
            },
            {
              "name": "Snake",
              "id": "36",
              "img": ""
            },
            {
              "name": "Ike",
              "id": "37",
              "img": ""
            },
            {
              "name": "Pokemon Trainer",
              "id": "38",
              "img": ""
            },
            {
              "name": "Diddy Kong",
              "id": "39",
              "img": ""
            },
            {
              "name": "Lucas",
              "id": "40",
              "img": ""
            },
            {
              "name": "Sonic",
              "id": "41",
              "img": ""
            },
            {
              "name": "King Dedede",
              "id": "42",
              "img": ""
            },
            {
              "name": "Olimar",
              "id": "43",
              "img": ""
            },
            {
              "name": "Lucario",
              "id": "44",
              "img": ""
            },
            {
              "name": "R.O.B.",
              "id": "45",
              "img": ""
            },
            {
              "name": "Toon Link",
              "id": "46",
              "img": ""
            },
            {
              "name": "Wolf",
              "id": "47",
              "img": ""
            },
            {
              "name": "Villager",
              "id": "48",
              "img": ""
            },
            {
              "name": "Mega Man",
              "id": "49",
              "img": ""
            },
            {
              "name": "Wii Fit Trainer",
              "id": "50",
              "img": ""
            },
            {
              "name": "Rosalina & Luma",
              "id": "51",
              "img": ""
            },
            {
              "name": "Little Mac",
              "id": "52",
              "img": ""
            },
            {
              "name": "Greninja",
              "id": "53",
              "img": ""
            },
            {
              "name": "Palutena",
              "id": "54",
              "img": ""
            },
            {
              "name": "Pac-Man",
              "id": "55",
              "img": ""
            },
            {
              "name": "Robin",
              "id": "56",
              "img": ""
            },
            {
              "name": "Shulk",
              "id": "57",
              "img": ""
            },
            {
              "name": "Bowser Jr.",
              "id": "58",
              "img": ""
            },
            {
              "name": "Duck Hunt Duo",
              "id": "59",
              "img": ""
            },
            {
              "name": "Ryu",
              "id": "60",
              "img": ""
            },
            {
              "name": "Ken",
              "id": "61",
              "img": ""
            },
            {
              "name": "Cloud",
              "id": "62",
              "img": ""
            },
            {
              "name": "Corrin",
              "id": "63",
              "img": ""
            },
            {
              "name": "Bayonetta",
              "id": "64",
              "img": ""
            },
            {
              "name": "Inkling",
              "id": "65",
              "img": ""
            },
            {
              "name": "Ridley",
              "id": "66",
              "img": ""
            },
            {
              "name": "Simon",
              "id": "67",
              "img": ""
            },
            {
              "name": "Richter",
              "id": "68",
              "img": ""
            },
            {
              "name": "King K. Rool",
              "id": "69",
              "img": ""
            },
            {
              "name": "Isabelle",
              "id": "70",
              "img": ""
            },
            {
              "name": "Incineroar",
              "id": "71",
              "img": ""
            },
            {
              "name": "Piranha Plant",
              "id": "72",
              "img": ""
            },
            {
              "name": "Joker",
              "id": "73",
              "img": ""
            },
            {
              "name": "Hero",
              "id": "74",
              "img": ""
            },
            {
              "name": "Banjo & Kazooie",
              "id": "75",
              "img": ""
            },
            {
              "name": "Terry",
              "id": "76",
              "img": ""
            },
            {
              "name": "Byleth",
              "id": "77",
              "img": ""
            },
            {
              "name": "Mii Brawler",
              "id": "78",
              "img": ""
            },
            {
              "name": "Mii Swordfighter",
              "id": "79",
              "img": ""
            },
            {
              "name": "Mii Gunner",
              "id": "80",
              "img": ""
            }
          ]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
