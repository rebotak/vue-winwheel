# vue-winwheel
a winwheel for vuejs based on http://dougtesting.net/home


published on: https://www.npmjs.com/package/vue-winwheel

# Demo

The demo page is [HERE](http://rebotak.github.io/vue-winwheel/demo.html). or maybe just download this repository and try the `demo.html` file

# Installation

## npm

```shell
$ npm install vue-winwheel
```

# Usage

## Basic

```html
  <vue-winwheel
    :segments="options"
    :wheelSize="wheelSize"
    :pageTitle="pageTitle"
    :lineWidth="lineWidth"
  />
```

```
<script>
import VueWinwheel from './VueWinwheel.vue'

export default {
  data(){
    return{
      wheelSize: 310,
      pageTitle: 'Vue-Wheel'
      lineWidth: 3,
      options:[
					{
						textFillStyle: '#fff',
						fillStyle: '#000',
						text:'Prize 1'
					},
					{
						textFillStyle: '#000',
						fillStyle: '#fadede',
						text:'Prize 2'
					},
					{
						textFillStyle: '#fff',
						fillStyle: '#000',
						text:'Prize 3'
					},
					{
						textFillStyle: '#000',
						fillStyle: '#fadede',
						text:'Prize 4'
					},
					{
						textFillStyle: '#fff',
						fillStyle: '#000',
						text:'Prize 5'
					},
					{
						textFillStyle: '#000',
						fillStyle: '#fadede',
						text:'Prize 6'
					},
					{
						textFillStyle: '#fff',
						fillStyle: '#000',
						text:'Prize 7'
					},
					{
						textFillStyle: '#000',
						fillStyle: '#fadede',
						text:'Prize 8'
					}
				]
    }
  }
}
</script>
```

# License

[The MIT License](http://opensource.org/licenses/MIT)
