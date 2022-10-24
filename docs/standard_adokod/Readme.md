Köszönjük a tervezettel kapcsolatos véleményeket, javaslatokat. A tervezetet mindezek figyelembevételével fogjuk kiegészíteni, amelyről visszajelzést fogunk adni a GitHub-on. A tervezettel kapcsolatban több jelzést és javaslatot is kaptunk a standard adókódok képzésével kapcsolatban. A NAV által tervezett standard adókódokat a mai napon a GitHub-on publikáltuk és szintén várjuk a véleményeket, javaslatokat.

Az eÁfa rendszer standard adókód képzéséhez az Adóhivatal kialakított egy olyan, általános, a jövőben bővíthető, illetve a változásokat követni tudó kódolási rendszert, amely alapján egy a bizonylaton szereplő információról egyértelműen megadható, hogy az a jelenlegi áfabevallásban milyen sorban vagy sorokban szerepeltetendő, illetve milyen adókulcshoz tartozik.
A standard adókód lehetőséget biztosít arra, hogy az adott adókódhoz további információkat, jelzéseket kapcsoljunk, ami által az adókódolt információt tovább lehet finomítani.

Az adóhatóság a standard adókód táblázatot fixnek tekinti, tehát az eÁfa rendszerben kizárólag az éppen aktuális standard adókódok szerepeltethetők. Azonban ügyféli javaslatok alapján a standard adókódlista bővíthető. 

A standard adókódok mellett célszerűnek látja az Adóhivatal beszédes elnevezés bevezetését is, amely valamilyen szempontrendszer alapján a felhasználók számára könnyű azonosíthatósgot jelet a részletes leírás és adókód mellett. A standard adókódok beszédes elnevezésére és módjára javaslatot várunk a GitHub fórumon keresztül. Kérjük a javaslatokat Ötletek kategóriában szerepeltessék.

Az adóhivatali standard adókód az alábbi logikai szerint épül fel.

A standard adókód elemei

•	MPxxx -> Fizetendő fő sor (Main Payable row), ahol az xxx a fősor száma
•	DPxxx -> Fizetendő Részletező sor (Detailed Payable row) ahol az xxx a részletező sor száma 
•	MDxxx -> Levonható fő sor (Main Deductable row) ahol az xxx a fősor száma 
•	DDxxx -> Levonható Részletezősor (Detailed Deductable row) ahol az xxx a részletező sor száma
•	DHxxx -> Részletező kiemelő sor (Detailed Highlight row) ahol az xxx a részletező kiemelő sor száma
•	PGxxx -> Lap (PaGe) -> ahol az xxx a Lap számát megneveztését tartalmazza pl PGA88
•	Kxxx -> Kulcs (Key) -> Kulcs-érték pár kulcs eleme 
•	Vxxx -> Érték (Value) -> Kulcs-érték pár érték eleme


A standard adókód kiértékelése
A standard adókódot egy kódelemekből álló halmaznak tekintjük. Ennek a halmaznak az elemeit vizsgáljuk, tartalmuk szerint.

Értelmezés
XX n, ahol XX a JELÖLÉS n pedig a lehetséges előfordulás darabszáma.

Példa:
MP n = 0 sor  jelentése: MP-vel kezdődő kód nincs a halmazban
DP n = 0,1,2,3 sor jelentése : DP-vel kezdődő kód előfordulása a halmazban nulla, egy, kettő, vagy három elemű lehet

Szabályok

Fizetendő oldal:
Ha MP n = 0 
akkor
DP n = 0
MD n = 1
DD n = 0,1
DH n = 0,1,2
PG n = 0,1
K n = 0,1 (ha K n = 0 akkor V n is = 0)
V n = 0,1 (ha V n = 0 akkor K n is = 0)

Ha MP n = 1 
akkor
DP n = 0,1,2,3
MD n = 1
DD n = 0,1
DH n = 0
PG n = 0,1
K n = 0,1 (ha K n = 0 akkor V n is = 0)
V n = 0,1 (ha V n = 0 akkor K n is = 0)

Ha MP n = 2 
akkor
DP n = 1
MD n = 1,0
DD n = 0 
DH n = 0
PG n = 0,1
K n = 0,1 (ha K n = 0 akkor V n is = 0)
V n = 0,1 (ha V n = 0 akkor K n is = 0)

Levonható oldal:

Ha MD n = 0 
akkor
DD n = 0 
MP n = 1
DP n = 0,1,2,3
DH n = 0,1,2
PG n = 0,1
K n = 0,1 (ha K n = 0 akkor V n is = 0)
V n = 0,1 (ha V n = 0 akkor K n is = 0)

Ha MD n = 1 
akkor
DD n = 0,1
MP n = 0,1
DP n = 0,1
DH n = 0
PG n = 0,1
K n = 0,1 (ha K n = 0 akkor V n is = 0)
V n = 0,1 (ha V n = 0 akkor K n is = 0)

Fentiek kombinációja: 
Ha MP n = 1 és MD n = 1 
akkor
DP n = 0,1,2
DD n = 0,1
DH n = 0
PG n = 0,1
K n = 0,1 (ha K n = 0 akkor V n is = 0)
V n = 0,1 (ha V n = 0 akkor K n is = 0)  
