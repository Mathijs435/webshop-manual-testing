# Fehlerberichte (Bug Reports) – Demo Webshop

In diesem Dokument werden alle während der Testdurchführung identifizierten Abweichungen (Defects) dokumentiert.

---

## BUG-01: Warenkorb-Persistenz nach Reload (Analyse)
**Status:** Abgelehnt (Closed / Not a Bug)  
**Schweregrad:** -  
**Priorität:** -  
**Titel:** Warenkorb bleibt nach Seiten-Reload gefüllt  
**Analyse:** Ursprünglich als Fehler vermutet, da der Warenkorb nach Drücken von F5 nicht geleert wurde. Nach Überprüfung der gängigen E-Commerce-Standards und der technischen Implementierung (LocalStorage) wurde festgestellt, dass dies ein gewünschtes Verhalten (Persistence) ist, um die User Experience zu verbessern.  
**Ergebnis:** Kein Fehler, das System verhält sich wie vorgesehen.

---

## BUG-02: Fehlendes Auto-Scrolling bei Paginierung
**Status:** Offen (Open)  
**ID:** BUG-002  
**Schweregrad:** Niedrig (UI/UX-Problem)  
**Priorität:** Mittel  
**Umgebung:** Chrome Version 120.0.x, Windows 11  
**Titel:** Seite scrollt nach Klick auf „Next“ nicht automatisch nach oben  

**Schritte zur Reproduktion:** 1. Die Startseite des Demo-Shops öffnen.  
2. Nach ganz unten scrollen, bis die Produktliste endet.  
3. Auf die Schaltfläche „Next“ klicken, um die nächste Seite zu laden.  

**Erwartetes Ergebnis:** Die neue Seite wird geladen und der Fokus (Viewport) springt automatisch an den Anfang der Seite, damit der Nutzer die neuen Produkte sofort sieht.  

**Tatsächliches Ergebnis:** Die neuen Produkte werden geladen, aber die Scroll-Position bleibt am Ende der Seite stehen. Der Nutzer muss manuell nach oben scrollen.  

**Vorschlag zur Behebung:** Ein `window.scrollTo(0, 0);` Call sollte nach dem erfolgreichen Laden der nächsten Produktseite ausgeführt werden.

---

## BUG-03: [Platzhalter für zukünftige Fehler]
*Hier werden weitere Fehler dokumentiert, sobald sie identifiziert werden.*

