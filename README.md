CSS
Alapbeállítások:

Minden elem nullázva van: nincs margó és padding, a box-sizing: border-box; az elemek méretezését kezeli.
A betűtípus a Poppins Google Fonts-ról van importálva.
Fejléc és navigáció stílusai:

A header szélessége 100%, magassága 50px, a háttér világos szürke. A tartalom középre igazított (flex használatával).
A .Logo sötét szürke színnel és nagyobb betűmérettel jelenik meg.
Navigációs menü:

A .nav ol flexbox elrendezést használ, hogy vízszintesen jelenítse meg a listaelemeket. Nincs felsorolásjel.
A menüpontok (<li> és <a>) stílusai tartalmaznak margókat, paddinget és kör alakú sarkokat, valamint egy átmenetet a hover eseményre.
Hamburger menü (kis kijelzőkre):

A checkbox (input) egy class="btn" osztályhoz kapcsolódik. Ez a checkbox egyáltalán nem látható (display: none;), kivéve mobil méretben.
A btn::before egy speciális tartalommal rendelkező pseudo-elemet hoz létre (itt egy Font Awesome ikon jelenne meg a hamburger menü ikonjához).
Hover effektusok:

A menüpontok alatti csík (háttér) egy pseudo-elem (a::before), ami alapesetben nagyon vékony (scaleY(0.05)), de amikor a felhasználó az egérrel rámutat, a csík megnyúlik (scaleY(1.1)).
A színátmenet a menüpont alatt lineáris gradiens: sötét színekből áll (zöld és fekete árnyalatok).
Reszponzív rész
1200px alatti kijelzők:

Itt jelenik meg a hamburger menü (.btn). A menü most már nem vízszintes, hanem rejtett (transform: translateY(-110%)), és csak akkor jelenik meg, ha a checkbox be van jelölve (input
).
A checkbox bejelölésére a hamburger menü ikonja egy "X" ikonra vált.
700px alatti kijelzők:

A menü elemei (ol lista) függőlegesen igazodnak (flex-direction: column).