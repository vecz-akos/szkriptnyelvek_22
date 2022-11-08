# Pi megközelítése

Amikor Pythonban a pi-vel kell számolnunk, akkor a legbiztosabb mód, ha használjuk a `math` modul `pi` értékét. A következő feladatban azonban ez tiltva van.

Nézd meg [ezt a rövid videót](https://www.youtube.com/watch?v=ELetCV_wX_c), és a bemutatott módszert felhasználva próbáld megközelíteni a pi értékét! A közelítés legalább 2 tizedesjegyig egyezzen a pivel!

Próbáld optimalizálni a gyorsabb futás érdekében!

__Tipp:__ egy pontról könnyen megmondhatjuk a következő módszerrel, hogy egy adott körön belül van-e. A koordináta rendszerben egy 1 egység sugarú kör középpontja legyen az origó. Ha a pont origótól való távolága kisebb, mint 1 (tehát rövidebb a sugárnál), akkor a körön belül van a pont, különben kívül (az x és y koordináták ismeretében távolság az origótól: `math.sqrt(x*x + y*y)`).
