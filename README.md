<div align="center">

# TypeScript types for Adobe Products [![Build Status](https://travis-ci.org/pravdomil/Types-for-Adobe.svg)](https://travis-ci.org/pravdomil/Types-for-Adobe)

Repository for declaration files generated by [extendscript-xml-to-typescript converter](https://github.com/pravdomil/extendscript-xml-to-typescript).

[<img src="https://i.imgur.com/VMx9MeE.jpg" width="560" height="315" />](http://youtu.be/h-c7A8pQzx8)

![gif](resources/gif.gif)

</div>

## Prerequisites
Install [Node.js](https://nodejs.org/en/download/) and [TypeScript](https://www.typescriptlang.org/#download-links) and git.

## Your first script for eg. Adobe Illustrator
```bash
# create new folder
mkdir my-script
cd my-script

# install types-for-adobe
npm init -y
npm i types-for-adobe

# create tsconfig.json
printf '{"compilerOptions":{"module":"none","noLib":true}}' > tsconfig.json

# create index.ts and change reference types to Adobe product you're targeting
printf '/// <reference types="types-for-adobe/illustrator/2015.3"/>\nalert(String(app));\n' > index.ts

# compile typescript files
tsc

# open Adobe Illustrator -> File -> Scripts -> Other Script -> and open index.js
 
```

## More typings

- [Adobe's offical typings](https://github.com/Adobe-CEP/Samples/tree/master/TypeScript/typings)
- [BrightShadow/CSInterface-TS](https://github.com/BrightShadow/CSInterface-TS)
- [Premiere](https://gitcdn.xyz/repo/Adobe-CEP/Samples/master/PProPanel/payloads/api_doc.html)

## Contributors
Thanks to [vespakoen](https://github.com/vespakoen), [atarabi](https://github.com/atarabi), [lm913](https://github.com/lm913).

## Contributing
Open pull request and be sure that:
- additional types are prefixed with underscore
- follow [resources/tslint.json](resources/tslint.json)

## Showcase
- [Pravdomil scripts for InDesign](https://github.com/pravdomil/Pravdomil-scripts-for-InDesign#readme)

## Become a backer
Support this project by [buying a beer](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=BCL2X3AFQBAP2&item_name=types-for-adobe%20Beer).
