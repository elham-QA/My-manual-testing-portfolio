# Login-Seite testen - Saucedemo

Ich habe die Login-Seite von Saucedemo getestet.  
Hier sind die Testfälle, die ich für erfolgreiche und fehlgeschlagene Logins geschrieben habe.

---

## TC-01: Erfolgreicher Login
Was ich testen möchte:  
Der Benutzer kann sich mit korrektem Benutzername und Passwort anmelden.

Schritte:  
1. Benutzername eingeben: standard_user  
2. Passwort eingeben: secret_sauce  
3. Auf Login klicken  

Erwartetes Ergebnis:  
Der Benutzer landet auf der Produktseite.

---

## TC-02: Falsches Passwort
Was ich testen möchte:  
Das System zeigt einen Fehler, wenn das Passwort falsch ist.

Schritte:  
1. Benutzername: standard_user  
2. Passwort: irgendwas Falsches  
3. Auf Login klicken  

Erwartetes Ergebnis:  
Fehlermeldung: "Username and password do not match"

---

## TC-03: Falscher Benutzername
Was ich testen möchte:  
Das System zeigt einen Fehler, wenn der Benutzername falsch ist.

Schritte:  
1. Benutzername: wrong_user  
2. Passwort: secret_sauce  
3. Auf Login klicken  

Erwartetes Ergebnis:  
Fehlermeldung: "Username and password do not match"

---

## TC-04: Benutzername ist leer
Was ich testen möchte:  
Das System fordert den Benutzernamen an, wenn das Feld leer ist.

Schritte:  
1. Benutzername leer lassen  
2. Passwort: secret_sauce  
3. Auf Login klicken  

Erwartetes Ergebnis:  
Fehlermeldung: "Username is required"

---

## TC-05: Passwort ist leer
Was ich testen möchte:  
Das System fordert das Passwort an, wenn das Feld leer ist.

Schritte:  
1. Benutzername: standard_user  
2. Passwort leer lassen  
3. Auf Login klicken  

Erwartetes Ergebnis:  
Fehlermeldung: "Password is required"

---

## TC-06: Beide Felder sind leer
Was ich testen möchte:  
Das System fordert zuerst den Benutzernamen an.

Schritte:  
1. Beide Felder leer lassen  
2. Auf Login klicken  

Erwartetes Ergebnis:  
Fehlermeldung: "Username is required"


## TC-07: Beide Felder leer – Prüfung der Fehlermeldungs-Reihenfolge
Was ich gemacht habe:  
Ich habe beide Felder (Benutzername und Passwort) leer gelassen und auf "Login" geklickt.

Ergebnis:  
Das System zeigt die Meldung: "Username is required"

Meine Anmerkung als Tester:  
Die Website prüft zuerst das Benutzername-Feld und stoppt dann.  
Es wäre benutzerfreundlicher, wenn eine kombinierte Meldung käme wie:  
"Benutzername und Passwort sind erforderlich".

Ist das ein Bug?  
Nein, kein Bug. Es ist so designed.  
Ich sehe es als Verbesserungsvorschlag (Improvement Suggestion) für eine bessere User Experience.

---

Hinweis: Das sind grundlegende Login-Tests. Ich kann bei Bedarf mehr Grenzfälle hinzufügen.
