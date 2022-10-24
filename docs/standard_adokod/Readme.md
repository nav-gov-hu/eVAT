<html>

<head>
<meta http-equiv=Content-Type content="text/html; charset=windows-1250">
<meta name=Generator content="Microsoft Word 15 (filtered)">


</head>

<body lang=HU style='word-wrap:break-word'>

<div class=WordSection1>

<p class=MsoNormal style='text-align:justify'>Köszönjük a tervezettel
kapcsolatos véleményeket, javaslatokat. A tervezetet mindezek figyelembevételével
fogjuk kiegészíteni, amelyről visszajelzést fogunk adni a GitHub-on. A
tervezettel kapcsolatban több jelzést és javaslatot is kaptunk a standard adókódok
képzésével kapcsolatban. A NAV által tervezett standard adókódokat a mai napon
a GitHub-on publikáltuk és szintén várjuk a véleményeket, javaslatokat.</p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'>Az eÁfa rendszer standard adókód
képzéséhez az Adóhivatal kialakított egy olyan, általános, a jövőben bővíthető,
illetve a változásokat követni tudó kódolási rendszert, amely alapján egy a
bizonylaton szereplő információról egyértelműen megadható, hogy az a jelenlegi
áfabevallásban milyen sorban vagy sorokban szerepeltetendő, illetve milyen adókulcshoz
tartozik.</p>

<p class=MsoNormal style='text-align:justify'>A standard adókód lehetőséget
biztosít arra, hogy az adott adókódhoz további információkat, jelzéseket
kapcsoljunk, ami által az adókódolt információt tovább lehet finomítani.</p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'>Az adóhatóság a standard adókód
táblázatot fixnek tekinti, tehát az eÁfa rendszerben kizárólag az éppen
aktuális standard adókódok szerepeltethetők. Azonban ügyféli javaslatok alapján
a standard adókódlista bővíthető. </p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'>A standard adókódok mellett
célszerűnek látja az Adóhivatal beszédes elnevezés bevezetését is, amely valamilyen
szempontrendszer alapján a felhasználók számára könnyű azonosíthatósgot jelet a
részletes leírás és adókód mellett. <b>A standard adókódok beszédes
elnevezésére és módjára javaslatot várunk a GitHub fórumon keresztül. </b>Kérjük
a javaslatokat <b>Ötletek</b> kategóriában szerepeltessék.</p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'>Az adóhivatali standard adókód az
alábbi logikai szerint épül fel.</p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'><b><u>A standard adókód elemei</u></b></p>

<p class=MsoNormal style='text-align:justify'><b>&nbsp;</b></p>

<p class=MsoListParagraphCxSpFirst style='text-align:justify;text-indent:-18.0pt'><span
style='font-family:Symbol'>·<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span>MPxxx -&gt; Fizetendő fő sor (Main Payable row), ahol az xxx a
fősor száma</p>

<p class=MsoListParagraphCxSpMiddle style='text-align:justify;text-indent:-18.0pt'><span
style='font-family:Symbol'>·<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span>DPxxx -&gt; Fizetendő Részletező sor (Detailed Payable row) ahol
az xxx a részletező sor száma </p>

<p class=MsoListParagraphCxSpMiddle style='text-align:justify;text-indent:-18.0pt'><span
style='font-family:Symbol'>·<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span>MDxxx -&gt; Levonható fő sor (Main Deductable row) ahol az xxx a
fősor száma </p>

<p class=MsoListParagraphCxSpMiddle style='text-align:justify;text-indent:-18.0pt'><span
style='font-family:Symbol'>·<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span>DDxxx -&gt; Levonható Részletezősor (Detailed Deductable row)
ahol az xxx a részletező sor száma</p>

<p class=MsoListParagraphCxSpMiddle style='text-align:justify;text-indent:-18.0pt'><span
style='font-family:Symbol'>·<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span>DHxxx -&gt; Részletező kiemelő sor (Detailed Highlight row) ahol
az xxx a részletező kiemelő sor száma</p>

<p class=MsoListParagraphCxSpMiddle style='text-align:justify;text-indent:-18.0pt'><span
style='font-family:Symbol'>·<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span>PGxxx -&gt; Lap (PaGe) -&gt; ahol az xxx a Lap számát
megneveztését tartalmazza pl PGA88</p>

<p class=MsoListParagraphCxSpMiddle style='text-align:justify;text-indent:-18.0pt'><span
style='font-family:Symbol'>·<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span>Kxxx -&gt; Kulcs (Key) -&gt; Kulcs-érték pár kulcs eleme </p>

<p class=MsoListParagraphCxSpLast style='text-align:justify;text-indent:-18.0pt'><span
style='font-family:Symbol'>·<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span>Vxxx -&gt; Érték (Value) -&gt; Kulcs-érték pár érték eleme</p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'><b><u>A standard adókód kiértékelése</u></b></p>

<p class=MsoNormal style='text-align:justify'>A standard adókódot egy
kódelemekből álló halmaznak tekintjük. Ennek a halmaznak az elemeit vizsgáljuk,
tartalmuk szerint.</p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'><b><u>Értelmezés</u></b></p>

<p class=MsoNormal style='text-align:justify'>XX n, ahol XX a JELÖLÉS n pedig a
lehetséges előfordulás darabszáma.</p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'><b><u>Példa:</u></b></p>

<p class=MsoNormal style='text-align:justify'>MP n = 0 sor  jelentése: MP-vel
kezdődő kód nincs a halmazban</p>

<p class=MsoNormal style='text-align:justify'>DP n = 0,1,2,3 sor jelentése : DP-vel
kezdődő kód előfordulása a halmazban nulla, egy, kettő, vagy három elemű lehet</p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'><b><u>Szabályok</u></b></p>

<p class=MsoNormal style='text-align:justify'><b><u><span style='text-decoration:
 none'>&nbsp;</span></u></b></p>

<p class=MsoNormal style='text-align:justify'><i><u>Fizetendő oldal:</u></i></p>
<p class=MsoNormal style='text-align:justify'>&nbsp;</p>
<p class=MsoNormal style='text-align:justify'>Ha MP n = 0 </p>

<p class=MsoNormal style='text-align:justify'>akkor</p>

<p class=MsoNormal style='text-align:justify'>DP n = 0</p>

<p class=MsoNormal style='text-align:justify'>MD n = 1</p>

<p class=MsoNormal style='text-align:justify'>DD n = 0,1</p>

<p class=MsoNormal style='text-align:justify'>DH n = 0,1,2</p>

<p class=MsoNormal style='text-align:justify'>PG n = 0,1</p>

<p class=MsoNormal style='text-align:justify'>K n = 0,1 (ha K n = 0 akkor V n
is = 0)</p>

<p class=MsoNormal style='text-align:justify'>V n = 0,1 (ha V n = 0 akkor K n
is = 0)</p>
<p class=MsoNormal style='text-align:justify'>&nbsp;</p>
<p class=MsoNormal style='text-align:justify'>Ha MP n = 1 </p>

<p class=MsoNormal style='text-align:justify'>akkor</p>

<p class=MsoNormal style='text-align:justify'>DP n = 0,1,2,3</p>

<p class=MsoNormal style='text-align:justify'>MD n = 1</p>

<p class=MsoNormal style='text-align:justify'>DD n = 0,1</p>

<p class=MsoNormal style='text-align:justify'>DH n = 0</p>

<p class=MsoNormal style='text-align:justify'>PG n = 0,1</p>

<p class=MsoNormal style='text-align:justify'>K n = 0,1 (ha K n = 0 akkor V n
is = 0)</p>

<p class=MsoNormal style='text-align:justify'>V n = 0,1 (ha V n = 0 akkor K n
is = 0)</p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'>Ha MP n = 2 </p>

<p class=MsoNormal style='text-align:justify'>akkor</p>

<p class=MsoNormal style='text-align:justify'>DP n = 1</p>

<p class=MsoNormal style='text-align:justify'>MD n = 1,0</p>

<p class=MsoNormal style='text-align:justify'>DD n = 0 </p>

<p class=MsoNormal style='text-align:justify'>DH n = 0</p>

<p class=MsoNormal style='text-align:justify'>PG n = 0,1</p>

<p class=MsoNormal style='text-align:justify'>K n = 0,1 (ha K n = 0 akkor V n
is = 0)</p>

<p class=MsoNormal style='text-align:justify'>V n = 0,1 (ha V n = 0 akkor K n
is = 0)</p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'><i><u>Levonható oldal:</u></i></p>

<p class=MsoNormal style='text-align:justify'>Ha MD n = 0 </p>

<p class=MsoNormal style='text-align:justify'>akkor</p>

<p class=MsoNormal style='text-align:justify'>DD n = 0 </p>

<p class=MsoNormal style='text-align:justify'>MP n = 1</p>

<p class=MsoNormal style='text-align:justify'>DP n = 0,1,2,3</p>

<p class=MsoNormal style='text-align:justify'>DH n = 0,1,2</p>

<p class=MsoNormal style='text-align:justify'>PG n = 0,1</p>

<p class=MsoNormal style='text-align:justify'>K n = 0,1 (ha K n = 0 akkor V n
is = 0)</p>

<p class=MsoNormal style='text-align:justify'>V n = 0,1 (ha V n = 0 akkor K n
is = 0)</p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'>Ha MD n = 1 </p>

<p class=MsoNormal style='text-align:justify'>akkor</p>

<p class=MsoNormal style='text-align:justify'>DD n = 0,1</p>

<p class=MsoNormal style='text-align:justify'>MP n = 0,1</p>

<p class=MsoNormal style='text-align:justify'>DP n = 0,1</p>

<p class=MsoNormal style='text-align:justify'>DH n = 0</p>

<p class=MsoNormal style='text-align:justify'>PG n = 0,1</p>

<p class=MsoNormal style='text-align:justify'>K n = 0,1 (ha K n = 0 akkor V n
is = 0)</p>

<p class=MsoNormal style='text-align:justify'>V n = 0,1 (ha V n = 0 akkor K n
is = 0)</p>

<p class=MsoNormal style='text-align:justify'>&nbsp;</p>

<p class=MsoNormal style='text-align:justify'><i><u>Fentiek kombinációja: </u></i></p>

<p class=MsoNormal style='text-align:justify'>Ha MP n = 1 és MD n = 1 </p>

<p class=MsoNormal style='text-align:justify'>akkor</p>

<p class=MsoNormal style='text-align:justify'>DP n = 0,1,2</p>

<p class=MsoNormal style='text-align:justify'>DD n = 0,1</p>

<p class=MsoNormal style='text-align:justify'>DH n = 0</p>

<p class=MsoNormal style='text-align:justify'>PG n = 0,1</p>

<p class=MsoNormal style='text-align:justify'>K n = 0,1 (ha K n = 0 akkor V n
is = 0)</p>

<p class=MsoNormal style='text-align:justify'>V n = 0,1 (ha V n = 0 akkor K n
is = 0)  </p>

</div>

</body>

</html>
