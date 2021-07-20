# Vue WinWheel

A wheel component for Vue 2.x based on http://dougtesting.net/home

Published on: https://www.npmjs.com/package/vue-winwheel

This fork is based on https://github.com/rebotak/vue-winwheel. Most of the changes here involved some logic cleanup and changes to make some of the wheel properties optional.

# Demo

Download this repository
```shell
git clone git@github.com:cshomo11/vue-winwheel.git
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
