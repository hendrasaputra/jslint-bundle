Installation
------------
1. Install hammerjs

		git clone http://github.com/senchalabs/hammerjs.git
		cd hammerjs
		cmake ./
		make	
	
2. Copy binary `hammerjs` ke PATH (e.g. /usr/local/bin)

		cp ./hammerjs /usr/local/bin
	
3. Copy `lint.js` dari folder `hammerjs/examples` ke PATH

		cp ./examples/lint.js /usr/local/bin
	
4. Buat shell script untuk wrapper jslint dengan isi sebagai berikut

		#!/bin/bash
		/usr/local/bin/hammerjs /usr/local/bin/lint.js $1
	
5. Pindah ke directory Bundle TextMate

		cd ~/Library/Application\ Support/TextMate/Bundles
		
6. Ambil jslint-bundle dari github
		
		git clone https://github.com/hendrasaputra/jslint-bundle.git
		
7. Reload Bundles on TextMate