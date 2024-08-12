
Verify bitcoin address signature online
address:
114oR4xdWh47GbXjP8TuN5VjyGFHkSJkDX
message:
cHNidP8BAP3mAQIAAAAKDQcRjIrfOk4YaTTn9M0Lae3DIFqNQbL0pLx/KTsrbghVAAAAAP3///+P65xghyjefjPCQLWhdnN8rFo1wtIClJyJxxi0aYeUJSIAAAAA/f///8THN/gzhXxj259zQE9takyRPTZENvGp71AiKKyJSmcqDgAAAAD9////siW/PnDV7UluLsx9oQ3mYrxQBDJMgfpjnpYHfZ0b2E8UAAAAAP3///9W9RBRv2cAfvYaQJm+/o9DpYrhuJ+nWJ+kKVGxA3uJaA0AAAAA/f///8kflw9nDTxPVB+l6d9iMlOR1ODN4NwaneOYxxE2lHV/QQAAAAD9////wF+In6DrLlKYH0ZQwsYQfS3iCodTS+t/NB6jEitgUstGAAAAAP3///8OjgPH7GW3J7P5kvprVGbrtqcxKk/Zo7uRvR5gdpT2zE8AAAAA/f///3vW8Cb7YNOBZk5n2ZVVu0tuQDU1TuhqGeqeBd9vkXLdAAAAAAD9////1vVLGdhhaq0DDQzAARzCGStpD0+5OT7tEdW8HjjkJ+o3AAAAAP3///8CaMMpAAAAAAAXqRQ2eygRsKicwIr+k31rNC8ddVNfBocgQCwAAAAAABl2qRQAt/4/JyqfGbUM8PLfgwYIK5HcKIisvA8NAAABASD5ChIAAAAAABepFDZ7KBGwqJzAiv6TfWs0Lx11U18GhwABASC/LwQAAAAAABepFDZ7KBGwqJzAiv6TfWs0Lx11U18GhwABASDM2AAAAAAAABepFDZ7KBGwqJzAiv6TfWs0Lx11U18GhwABASDLMgMAAAAAABepFDZ7KBGwqJzAiv6TfWs0Lx11U18GhwABASCL/AEAAAAAABepFDZ7KBGwqJzAiv6TfWs0Lx11U18GhwABASC5uwgAAAAAABepFDZ7KBGwqJzAiv6TfWs0Lx11U18GhwABASCSTQIAAAAAABepFDZ7KBGwqJzAiv6TfWs0Lx11U18GhwABASCkDAQAAAAAABepFDZ7KBGwqJzAiv6TfWs0Lx11U18GhwABASBj9wMAAAAAABepFDZ7KBGwqJzAiv6TfWs0Lx11U18GhwABASDFzSYAAAAAABepFDZ7KBGwqJzAiv6TfWs0Lx11U18GhwAAAA==
signature:
HH7p3lkrxCUhdbPt6cROK3QckppccaAmHbTwnh53HIwrN5hHVaH6fOKjW3eoAWFeHEoCi2IkBmMamDYsLZZmgvM=

address has 0 BTC

Signature verified!


This page works offline. Fork me on Github!
Verify bitcoin address signature online
Verify bitcoin address signature online
=======================================

Why? Because none of the existing pages on the interwebs are good. None of them could accept all the data via get parameters, 
and none of them were easily forkable to be hosted independently.
    
This implementation can accept get parameters, so it is linkable externally, and users could easily copy-paste one link to their counterparties to verify. 
This should be useful for people who do OTC and regularly do proof-of-funds before the transaction.

Try it
------

* hosted on https://bluewallet.github.io/VerifySignature
* or try with get parameters: https://bluewallet.github.io/VerifySignature?a=1HvaxYmChk9nQUZx888a6hc7E8KnKP98ic&m=test&s=HCfgnEo8RNYTgcOXafAf11BQQ5LXSvlss0AbnezENbFJQzRl0dJRGOfYbOrOPkb2iPdj21Cty5G4paevOks%2FpJ4%3D
* ...or short it https://bit.ly/3Gm85si

Built with
----------

* Next.js
* Bitcoinjs
* Typescript
* Blockstream API (address balance)
* ..compiles into static html files so it can run completely offline

![image](https://user-images.githubusercontent.com/1913337/127367603-0bff2674-07f0-4a4f-846d-b3a6fc7860db.png)


Build it yourself
-----------------

```js
npm i
npm run export
```

And it is ready to be hosted on the website (should be served from `/VerifySignature/` path, i.e. `http://localhost:3000/VerifySignature`).
Use `npm run dev` for development.

License
-------

MIT
