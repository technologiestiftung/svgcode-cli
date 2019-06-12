# CLI for @tsb/svgcode

## Install

```bash
npm install @tsb/svgcode-cli -g
```

## Usage

```bash
  Usage: svgcode ./path/to/infile.svg [./path/to/outfile.gc] [FLAGS]

  Options:
    -c --config {string} Path to config.json
    -d --dedupe {boolean} Default true removes following duplicate lines from gcode
    -f --feedrate {number} Default 3125 Feedrate to write to top of gcode
    --floor {boolean} Default true Removes .000 values from coordinates
    --print {boolean} Default false Prints the Gcode after generation

  Config (needs valid json overrules cli flags):
  {
    "depth": 10,
    "map": "xyz",
    "precision": 1,
    "ramping": false,
    "toolDiameter": 1,
    "top": -10,
    "unit": "mm",
    "floor": false,
    "dedupe": true,
    "feedrate": 3000,
    "print": false
  }
```

## Related

- [@tsb|svgcode the library used](https://github.com/technologiestiftung/svgcode)
- [@tsb/substrate cli for generating SVG graphics](https://github.com/technologiestiftung/substrate)
- [Original repo by piLeoni](https://github.com/piLeoni/svgcode)

## License

MIT License

Copyright (c) 2019 Technologiestiftung Berlin & Fabian Morón Zirfas

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

