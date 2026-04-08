# Testfälle – Demo Webshop

## Testfall 1: Produkt in den Warenkorb legen
**Ziel:** Sicherstellen, dass ein Produkt korrekt in den Warenkorb gelegt wird.  
**Voraussetzungen:** Webshop ist geöffnet.  
**Schritte:**  
1. Ein beliebiges Produkt auswählen  
2. Auf „In den Warenkorb“ klicken  
3. Warenkorb öffnen  
**Erwartetes Ergebnis:**  
Produkt erscheint im Warenkorb mit korrektem Namen, Preis und Menge.

---

## Testfall 2: Produkt aus dem Warenkorb entfernen
**Ziel:** Sicherstellen, dass Produkte korrekt entfernt werden.  
**Voraussetzungen:** Mindestens ein Produkt befindet sich im Warenkorb.  
**Schritte:**  
1. Warenkorb öffnen  
2. Auf „Entfernen“ oder „Löschen“ klicken  
**Erwartetes Ergebnis:**  
Produkt verschwindet aus dem Warenkorb. Warenkorb zeigt korrekten Gesamtpreis an.

---

## Testfall 3: Menge eines Produkts ändern
**Ziel:** Überprüfen, ob die Mengenänderung korrekt funktioniert.  
**Voraussetzungen:** Produkt liegt im Warenkorb.  
**Schritte:**  
1. Warenkorb öffnen  
2. Menge von „1“ auf „2“ erhöhen  
**Erwartetes Ergebnis:**  
Gesamtpreis aktualisiert sich korrekt.

---

## Testfall 4: Produktsuche verwenden
**Ziel:** Sicherstellen, dass die Suchfunktion relevante Ergebnisse liefert.  
**Schritte:**  
1. Suchfeld öffnen  
2. „Shirt“ oder ein anderes Produkt eingeben  
3. Enter drücken  
**Erwartetes Ergebnis:**  
Relevante Produkte werden angezeigt.

---

## Testfall 5: Fehlermeldung bei leerem Pflichtfeld im Checkout
**Ziel:** Überprüfen, ob der Checkout Pflichtfelder validiert.  
**Schritte:**  
1. Warenkorb öffnen  
2. Zur Kasse gehen  
3. Pflichtfelder leer lassen  
4. Auf „Weiter“ klicken  
**Erwartetes Ergebnis:**  
Eine klare Fehlermeldung erscheint (z. B. „Dieses Feld darf nicht leer sein“).

---

## Testfall 6: Preis auf Produktseite vs. Warenkorb vergleichen
**Ziel:** Sicherstellen, dass Preise konsistent sind.  
**Schritte:**  
1. Produktseite öffnen  
2. Preis merken  
3. Produkt in den Warenkorb legen  
4. Warenkorb öffnen  
**Erwartetes Ergebnis:**  
Preis ist identisch.
