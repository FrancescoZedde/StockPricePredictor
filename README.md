# StockPricePrediction
To predict stock prices. Features based on last values in a timestep, and technical indicators.

Currently running on https://price-predictor-eu.herokuapp.com/

On Windows 11, in case of this error after executing server node.js:
C:\laragon\www\StockPricePredictor
C:\laragon\www\StockPricePredictor
node:internal/modules/cjs/loader:1183
  return process.dlopen(module, path.toNamespacedPath(filename));
                 ^

Error: The specified module could not be found.
\\?\C:\laragon\www\StockPricePredictor\node_modules\@tensorflow\tfjs-node\lib\napi-v7\tfjs_binding.node
    at Object.Module._extensions..node (node:internal/modules/cjs/loader:1183:18)
    at Module.load (node:internal/modules/cjs/loader:981:32)
    at Function.Module._load (node:internal/modules/cjs/loader:822:12)
    at Module.require (node:internal/modules/cjs/loader:1005:19)
    at require (node:internal/modules/cjs/helpers:102:18)
    at Object.<anonymous> (C:\laragon\www\StockPricePredictor\node_modules\@tensorflow\tfjs-node\dist\index.js:58:16)
    at Module._compile (node:internal/modules/cjs/loader:1101:14)
    at Object.Module._extensions..js (node:internal/modules/cjs/loader:1153:10)
    at Module.load (node:internal/modules/cjs/loader:981:32)
    at Function.Module._load (node:internal/modules/cjs/loader:822:12) {
  code: 'ERR_DLOPEN_FAILED'
}


try to move tensorflow.dll
from .\StockPricePredictor\node_modules\@tensorflow\tfjs-node\deps\lib
to .\StockPricePredictor\node_modules\@tensorflow\tfjs-node\lib\napi-v7