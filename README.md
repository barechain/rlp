# rlp
Recursive Length Prefix Encoding in PHP.

[![Licensed under the MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/web3p/rlp/blob/master/LICENSE)

# Install

Set minimum stability to dev
```
composer require web3p/rlp
```

# Usage

RLP encode:
```
use RLP\RLP;

$rlp = new RLP;
$encodedBuffer = $rlp->encode(['dog']);

// to string, encoding: ascii utf8 hex
$encodedBuffer->toString($encoding);
```

RLP decode:
```
use RLP\RLP;

$rlp = new RLP;
$encodedBuffer = $rlp->encode(['dog']);

// only accept 0x prefixed hex string
$decodedArray = $rlp->decode('0x' . $encodedBuffer->toString('hex'));

// show dog
echo $decodedArray[0]->toString('utf8');
```

# API

Todo.

# License
MIT