# WiTI-Education--NodeJS-Certification--Capitulo-9

## Lab 9.1 - Single Use Listener
The labs-1index.jsfile contains the following code:
```javascript
'use strict'
const assert = require('assert')
const { EventEmitter } = require('events')const ee = new EventEmitter()let count = 0setInterval(() => {ee.emit('tick')}, 100)function listener () {count++setTimeout(() => {assert.equal(count, 1)assert.equal(this, ee)console.log('passed!')}, 250)}Register thelistenerfunction with theeeevent emitterin such a way that thelistenerfunction is only called a single time. If implemented correctly, the program should print outpassed!:LFW211           © Copyright the Linux Foundation 2020-2022. All rights reserved.
