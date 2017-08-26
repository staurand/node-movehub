# movehub

[![NPM version](https://badge.fury.io/js/movehub.svg)](http://badge.fury.io/js/movehub)
[![Dependency Status](https://img.shields.io/gemnasium/hobbyquaker/node-movehub.svg?maxAge=2592000)](https://gemnasium.com/github.com/hobbyquaker/node-movehub)
[![XO code style](https://img.shields.io/badge/code_style-XO-5ed9c7.svg)](https://github.com/sindresorhus/xo)
[![License][mit-badge]][mit-url]

> Node.js interface for the Lego Boost Move Hub

**WORK IN PROGRESS - UNFINISHED!**


## Install

```
$ npm install movehub
```


## TODO

- [x] LED control
- [ ] Motor control
- [ ] Sound playback
- [ ] Distance sensor events
- [ ] Color sensor events
- [ ] Rotation events
- [ ] Tilt sensor events
- [ ] Connect to multiple Move Hubs
- [ ] API Docs


## API

## Classes

<dl>
<dt><a href="#Boost">Boost</a></dt>
<dd></dd>
</dl>

## Functions

<dl>
<dt><a href="#Boost_disconnect
Disconnect from Move Hub">Boost:disconnect
Disconnect from Move Hub()</a></dt>
<dd></dd>
</dl>

## Events

<dl>
<dt><a href="#Boost_connect">"Boost:connect"</a></dt>
<dd></dd>
<dt><a href="#Boost_disconnect">"Boost:disconnect"</a></dt>
<dd></dd>
</dl>

<a name="Boost"></a>

## Boost
**Kind**: global class  

* [Boost](#Boost)
    * [.led(color, [callback])](#Boost+led)
    * ["scanning"](#Boost+event_scanning)
    * ["hub-found"](#Boost+event_hub-found)

<a name="Boost+led"></a>

### boost.led(color, [callback])
**Kind**: instance method of [<code>Boost</code>](#Boost)  

| Param | Type | Description |
| --- | --- | --- |
| color | <code>boolean</code> \| <code>number</code> \| <code>string</code> |  |
| [callback] | <code>function</code> | If set to boolean `false` the LED is switched off, if set to `true` the LED will be white. Possible string values: `off`, `pink`, `purple`, `blue`, `lightblue`, `cyan`, `green`, `yellow`, `orange`, `red`, `white` |

<a name="Boost+event_scanning"></a>

### "scanning"
reports when noble is starts/stops to scan for BLE devices

**Kind**: event emitted by [<code>Boost</code>](#Boost)  
<a name="Boost+event_hub-found"></a>

### "hub-found"
**Kind**: event emitted by [<code>Boost</code>](#Boost)  
**Properties**

| Name | Type |
| --- | --- |
| uuid | <code>string</code> | 
| address | <code>string</code> | 
| localName | <code>string</code> | 
| rssi | <code>number</code> | 

<a name="Boost_disconnect
Disconnect from Move Hub"></a>

## Boost:disconnect
Disconnect from Move Hub()
**Kind**: global function  
<a name="Boost_connect"></a>

## "Boost:connect"
**Kind**: event emitted  
<a name="Boost_disconnect"></a>

## "Boost:disconnect"
**Kind**: event emitted  


## Credits

Thanks to [Jorge Pereira](https://github.com/JorgePe) who analyzed and documented the move hub ble protocol:
https://github.com/JorgePe/BOOSTreveng


## License

MIT (c) Sebastian Raff

[mit-badge]: https://img.shields.io/badge/License-MIT-blue.svg?style=flat
[mit-url]: LICENSE
