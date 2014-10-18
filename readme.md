# node-dark-mode

> Toggle the [Dark Mode](http://www.macworld.co.uk/how-to/mac-software/turn-on-yosemites-dark-mode-on-mac-3534690/) in OS X 10.10 using the [dark-mode](https://github.com/sindresorhus/dark-mode) binary

![](https://github.com/sindresorhus/dark-mode/raw/master/screenshot.gif)


## Install

```sh
$ npm install --save dark-mode
```


## Usage

```js
var darkMode = require('dark-mode');

darkMode.toggle(function (err) {
	console.log('toggled between dark and light mode');
});

darkMode.toggle(true, function (err) {
	console.log('forced dark mode');
});
```


## API

### darkMode.toggle(force, callback)

#### force

Type: `boolean`  
Default: `null`

Force a specific mode, `true` for dark and `false` for light.

#### callback(error)

### darkMode.isDark(callback)

#### callback(error, isDark)

##### isDark

Type: `boolean`  

Whether the current mode is dark.


## CLI

```sh
$ npm install --global dark-mode
```

```sh
# toggle between dark and light mode
dark-mode

# force a specific mode
dark-mode --mode Dark
dark-mode --mode Light

# get the current mode
dark-mode --mode
> Light
```


## License

MIT © [Sindre Sorhus](http://sindresorhus.com)
