# YouTube timestamp generálás

YouTube videók leírásába van lehetőség timestampek elhelyezésére, ami segít eligazodni a videó különböző részei között. Például egy tutoriál esetén az általunk érdekelt részre ugorhatunk egyből. [Ennek a videónak](https://www.youtube.com/watch?v=4HJ_Nq6LOmk&ab) a leírásában vannak timestampek.

Az időbélyegek linkeit a YouTube a következőképpen generálja: a videó alap linkjéhez hozzácsatol egy lekérdezés paramétert `t` néven, aminek az értéke egy szám, ez a videó kezdetétől számítva jelzi az átugrandó másodperceket. Például, ha a timestamp egy sorának 01:15 értéket írunk, abban az esetben a videó elejétől számítva a 75. másodpercre ugrik. Ezzel az alap linkhez a következő paramétert adja hozzá: `t=75` (ezt megfigyelhetjük a fenti linken)

Azonban a timestampek szerkesztésekor még nem férünk hozzá a linkekhez, így ha ellenőrizni szeretnénk, akkor számolgatni kell a megfelelő másodperceket és begépelni az URL-t. Ennek megsegítésére kell írni programot.

A program kérjen bemnetként egy fájlt (amiben csak a timestampek vannak, soronként egy-egy, úgy, ahogy a videók leírásában) és a videó linkét (vagy esetleg a videó azonosítóját), majd készítse el minden sorhoz a megfelelő linket. Végül ez alapján generáljon le egy egyszerű HTML fájlt, amit mentsen el. Ebben legyenek a linkek, meg esetleg pár hasznos információ. A program ajánlja fel, hogy megnyitja böngészőben.

A HTML megnyitásához érdemes használni a standard könyvtárban található webbrowser modul `open_url` függvényét.

A feladat megoldása során lehetőleg használjuk a standard könyvtárat! A timestampeket más formákban is meg lehet adni, de elsődlegesen a példában megadott formát részesítjük előnyben (esetleg próbálhatunk univerzálisabb megoldást is adni).
