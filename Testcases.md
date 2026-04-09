# Testfälle – Demo Webshop (ISTQB-basiert)

Dieses Dokument enthält die funktionalen Testfälle für den Demo-Webshop. Jeder Testfall ist nach professionellen Standards strukturiert, um Nachvollziehbarkeit und Wiederholbarkeit zu gewährleisten.

---

## TC-01: Produkt in den Warenkorb legen
**Priorität:** Hoch  
**Ziel:** Sicherstellen, dass ein Produkt korrekt in den Warenkorb gelegt wird.  
**Voraussetzungen:** Der Webshop ist im Browser geöffnet.  
**Testdaten:** Produkt "Samsung Galaxy S6"  
**Schritte:** 1. Das Produkt "Samsung Galaxy S6" auf der Startseite auswählen.  
2. Auf die Schaltfläche „Add to cart“ klicken.  
3. Den Bestätigungs-Alert mit "OK" schließen.  
4. Den Link „Cart“ im Navigationsmenü öffnen.  
**Erwartetes Ergebnis:** Das Produkt erscheint in der Liste im Warenkorb mit dem korrekten Namen ("Samsung Galaxy S6") und dem entsprechenden Preis.

---

## TC-02: Produkt aus dem Warenkorb entfernen
**Priorität:** Mittel  
**Ziel:** Sicherstellen, dass Produkte korrekt entfernt werden.  
**Voraussetzungen:** Mindestens das Produkt "Samsung Galaxy S6" befindet sich im Warenkorb.  
**Schritte:** 1. Den Warenkorb („Cart“) öffnen.  
2. In der Zeile des Produkts auf den Link „Delete“ klicken.  
**Erwartetes Ergebnis:** Das Produkt verschwindet sofort aus der Liste. Der Warenkorb ist leer (oder zeigt die verbleibenden Produkte korrekt an).

---

## TC-03: Mengenänderung / Grenzwerttest
**Priorität:** Mittel  
**Ziel:** Überprüfen, ob die Mengenänderung und Preisaktualisierung korrekt funktioniert.  
**Voraussetzungen:** Ein Produkt liegt im Warenkorb.  
**Testdaten:** Menge = 2  
**Schritte:** 1. Den Warenkorb öffnen.  
2. Die Menge des Produkts von „1“ auf „2“ erhöhen (oder das Produkt ein zweites Mal hinzufügen).  
**Erwartetes Ergebnis:** Der Gesamtbetrag (Total) aktualisiert sich automatisch und zeigt die Summe beider Artikel korrekt an.

---

## TC-04: Produktsuche verwenden
**Priorität:** Mittel  
**Ziel:** Sicherstellen, dass die Suchfunktion relevante Ergebnisse liefert.  
**Schritte:** 1. Das Suchfeld in der Navigationsleiste anklicken.  
2. Den Suchbegriff „Laptop“ eingeben.  
3. Die Enter-Taste drücken oder auf das Lupe-Symbol klicken.  
**Erwartetes Ergebnis:** Die Ergebnisseite zeigt ausschließlich Produkte an, die den Begriff „Laptop“ im Titel oder in der Beschreibung enthalten.

---

## TC-05: Validierung von Pflichtfeldern im Checkout
**Priorität:** Hoch  
**Ziel:** Überprüfen, ob der Checkout-Prozess Pflichtfelder korrekt validiert.  
**Voraussetzungen:** Ein Produkt befindet sich im Warenkorb; der User ist im Checkout-Dialog ("Place Order").  
**Testdaten:** Alle Felder (Name, Land, Stadt) ausfüllen, aber das Feld „Credit card“ leer lassen.  
**Schritte:** 1. Auf die Schaltfläche „Purchase“ klicken.  
**Erwartetes Ergebnis:** Die Bestellung wird nicht abgeschlossen. Eine klare Fehlermeldung erscheint, die darauf hinweist, dass das Kreditkartenfeld ausgefüllt werden muss.

---

## TC-06: Preiskonsistenz prüfen
**Priorität:** Hoch  
**Ziel:** Sicherstellen, dass der Preis auf der Produktseite mit dem Preis im Warenkorb übereinstimmt.  
**Schritte:** 1. Die Detailseite des Produkts "Nokia lumia 1520" öffnen.  
2. Den angezeigten Preis notieren ($820).  
3. Das Produkt in den Warenkorb legen.  
4. Den Warenkorb („Cart“) öffnen.  
**Erwartetes Ergebnis:** Der im Warenkorb angezeigte Preis für das Produkt ist identisch mit dem Preis auf der Detailseite ($820).
