# vue-winwheel

a winwheel for vuejs based on http://dougtesting.net/home

published on: https://www.npmjs.com/package/vue-winwheel

# Demo

Download this repository
```shell
git clone git@github.com:rebotak/vue-winwheel.git
```

Go to the demo folder
```shell
/vue-winwheel/demo
```

Then install dependencies
```shell
npm install
```

And run the project
```shell
npm serve
```


# Installation

## npm

```shell
$ npm install vue-winwheel
```

# Usage

## Basic

```html
<VueWinwheel :segments="options" />
```

```
<script>
import VueWinwheel from 'vue-winwheel/vue-winwheel'

export default {
  components:{
    VueWinwheel
  },
  data(){
    return{
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
