# Smart Rack Configurator

Aplicație web (un singur fișier `index.html`, fără build și fără backend) pentru proiectarea rack-urilor și a documentației de cablare.

## Funcții
- Rack de la 4U la 48U, drag & drop sau click pe U-ul dorit, detecție de coliziuni, vedere față/spate
- Librărie pe categorii cu căutare și șabloane proprii (Switch, Router, Firewall, NVR, Server, Patch Panel, ODF, UPS, PDU, CATV, organizator cabluri etc.)
- Porturi cu destinație, locație, status, mod/VLAN, culoare cablu; ODF cu tip fibră și atenuare
- UPS cu intrări, ieșiri și grupuri (intrarea 1 = 220V); alimentare PDU și echipamente
- Conectare cablu între porturi (drag sau două click-uri), cu glow, capete de cablu spre organizator
- Live Cable Matrix editabil, pe echipamente, cu alegere de port din alt echipament
- Tab CATV (splittere, derivatoare, amplificatoare, prize)
- Calcul consum (W / BTU/h) vs. capacitate UPS
- Export Excel (câte o foaie pe echipament), PDF (cu imaginea rack-ului), imagine PNG, salvare/încărcare .json

## Publicare pe GitHub Pages
1. Creează un repository nou pe GitHub și încarcă toate fișierele din acest folder (inclusiv `.nojekyll`).
2. Settings → Pages → Source: *Deploy from a branch* → `main` / `(root)` → Save.
3. După ~1 minut aplicația e la `https://<utilizator>.github.io/<nume-repo>/`.

## Note
- Datele se salvează automat în browserul folosit (localStorage). Pentru backup sau mutare pe alt dispozitiv folosește „Salvează .json” / „Încarcă .json”.
- Exportul Excel și PDF folosește SheetJS, jsPDF și jsPDF-AutoTable încărcate de pe cdnjs, deci este nevoie de internet.
