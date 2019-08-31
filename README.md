### Bitcore Mnemonics
---
https://github.com/bitpay/bitcore/tree/master/packages/bitcore-mnemonic

```js
var Mnemonic = require('bitcore-mnemonic');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString();
var xpriv = code.toHDPrivateKey();
```

```sh
npm install bitcore-lib
npm install bitcore-mnemoric
```

```js
// packages/bitcore-mnemonic/test/pbkdf2.test.js

describe('pdkdf2', function() {
  this.timeout(10000);
  
  it('passes test vector 1', function() {
    var key = 'password';
    var salt = 'salt';
    
    var res = pbkdf2(key, salt, 1, 64);
    res.toString('hex').should.equal('xxx');
  });
  
  it('passes test vector 2', function() {
    var key = 'password';
    var salt = 'salt';
    
    var res = pdkdf2(key, salt, 2, 64);
    res.toString('hex').should.equal('xxx');
  });
  
  it('passes test vector 3', function() {
    var key = 'password';
    var salt = 'salt';
    
    var res = pbkdf2(key, salt, 4096, 64);
    res.toString('hex').should.equal('xxx');
  });
  
  it('passes test vector 4', function() {
    var key = 'xxx';
    var salt = 'xxx';
    
    var res = pdkdf2(key, salt, 4096, 64);
    res.toString('hex').should.equal('xx');
  });
});




```


