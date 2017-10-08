# Cryptoparty

## Es gibt keine Privatsphäre mehr, es gibt nur noch digitale Selbstverteidigung

Privatsphäre im politischen Struggle
* Trennung zwischen Public and Private (Hannah Arendt) als bürgerliches Ideal
* Problem: im privaten passiert viel Unterdrückung, zB häusliche Gewalt
  * Die kleinste Zelle des Faschismus ist die Kleinfamilie
* Wir wollen uns den öffentlichen Raum erobern
  * Ich will öffentlich Kleider tragen und Leute vögeln können, die ich mag
  * Eine Hautfarbe kann man nicht im privaten verstecken
  * Wenn Löhne intransparent sind, sind Arbeitskämpfe schwierig und Gender Pay Gap die Norm

Privatsphäre ist ein Recht, dass vom Staat gewährt wird
* Rechte können gegeben und genommen werden, nur wenn man sie erkämpft, sind sie was wert
* Autoritäre Staaten neigen dazu, ungenaue Gesetzeslagen zu haben;
  dann ist jeder ein bisschen schuldig, und du kannst die verknacken,
  die zu unbequem sind (Spoiler: Leute wie wir)

Es gibt keine Privatsphäre mehr, es gibt nur noch Verschlüsselung
* Daten für sich selbst können unschuldig sein, aber wir wissen nie, was sie aussagen können, wenn man sie vernetzt
* Wir können aber versuchen, zu verschlüsseln, um zumindest direkte Kommunikation unlesbar zu machen
* Verschlüsselung macht Überwachung teurer -> encrypt everything!

## PGP - Was ist asymmetrische Verschlüsselung?

Schlüsselpaar:
* Öffentlicher Schlüssel: den brauchen andere, um Nachrichten an euch verschlüsseln zu können
* Privater Schlüssel: den nutzt ihr, um Nachrichten zu entschlüsseln, die mit eurem öffentlichen Key verschlüsselt wurden.

Alice will Bob eine Email schicken:
* Alice fragt den Keyserver nach Bobs Public Key
* Alice verschlüsselt eine Email mit Bobs und ihrem eigenen Public Key
* Alice schickt die Email zu Bob
* Bob entschlüsselt die Email mit seinem Private Key
* Alice kann die Email auch in ihrem "Gesendet"-Ordner wieder ansehen, wenn sie sie entschlüsselt

Signieren
* Mit seinem Private Key kann man eine Nachricht signieren.
* Wie eine Unterschrift, nur dass sie mathematisch sicher ist (schwer zu fälschen)
* In Estland sind kryptographische Unterschriften rechtsgültig
* Eine Signatur ist keine Verschlüsselung!

## Der Kampf um das größte Netzwerk

Netzwerkeffekte
* Email hat fast jede\*r - größter Netzwerkeffekt überhaupt
* Bei anderen Netzwerken haben fast überall Monopole die Vorherrschaft; Facebook zB ist schwer zu verweigern
* Damit gibt man Plattformen Macht; Facebook, Google/Alphabet, Microsoft, Apple und Amazon sind die Big 5, mit exorbitanter Machtkonzentration
* Für Aktivistis ist es nicht nur ethisch schwierig, diese Monopolisierung zu unterstützen, es macht uns auch angreifbar für Zensur und Überwachung
* Ich bin die Freiheit des anderen; nur wenn ich viele verschiedene Dienste benutze, erlaube ich anderen, mich so zu kontaktieren, wie sie wollen

Dezentralität
* Beispiel: Email, Jabber
* Dezentralität wirkt Monopolisierung entgegen
* Die Kontrolle liegt bei dezentralen Diensten beim Admin des Servers

## Messenger im Vergleich

Whatsapp
* ist mittlerweile end2end-encrypted
* Hat sehr viele User (aber mich zB nicht :P)
* Contra: ist nicht open Source, und damit nicht vertrauenswürdig
* Wenn Whatsapp die Verschlüsselung abschaltet, würden wir das nicht mal merken
* Contra: ist nicht dezentral; die haben die Kontrolle über die Server
* Contra: Kann auf dem Desktop nur verwendet werden, wenn ein Smartphone gleichzeitig connected ist

**Wire**
* ist end2end-encrypted und mittlerweile open Source
* sehr schön designte App
  * Linux, Windows, Mac OS, Android, iOS, und im Browser
* Contra: ist (noch) nicht dezentral

Signal
* ist end2end-encrypted und open Source
* Wird von einer spendenfinanzierten NGO entwickelt
* Contra: Kann auf dem Desktop nur verwendet werden, wenn ein Smartphone gleichzeitig connected ist
* Contra: Entwickler stellen sich gegen Dezentralität

Telegram
* ist (schlecht) end2end-encrypted und open Source
* Der Entwickler hat sich öfters gegen Bestechungsversuche etc. vom FBI gewehrt
* Contra: Desktop-Client kann nicht E2E verschlüsseln
* Contra: der Algorithmus ist echt scheiße, sagen Kryptographen

XMPP/Jabber
* ist wie Email ein Protokoll, kein Service -> dh, sehr dezentral
* Es gibt Clients für alle möglichen Plattformen, die meisten können verschlüsseln.
  * Empfohlene Clients: Gajim für Desktop, Conversations für Android
* OTR: ist ein etwas älterer Standard, bei dem Nachrichten, die während einer Sitzung geschrieben werden,
  später nicht mehr lesbar sind
* Omemo: ist dasselbe Protokoll wie bei Wire, Whatsapp, und Signal
* Contra: Jabbers Gruppenkonversationen sind nicht so intuitiv

Autocrypt
* Autocrypt ist ein aufkommender Standart, der Messaging auf Basis von Email und PGP erleichtert.
* Mobile Client: Deltachat (sonst noch keine)
* Der PGP-Public-Key wird im Header mitgeschickt, statt auf nem Keyserver zu liegen
* Größte Userbase der Welt: fast jede\*r benutzt Email
* Contra: Noch kaum Clients, bisher nur Deltachat als mobile client

# Andere Lösungen:

Privnote.com
* Man schreibt die Nachricht in die Privnote und verschickt den Link an jmd.
* Die Nachricht wird, nachdem sie entschlüsselt wird, sofort gelöscht
* Gut, um mit Leuten zu kommunizieren, die zu faul für Crypto sind
* Leider etwas aufwändig für Massenmails etc.

# Dinge einrichten:

Nun der praktische Teil, das tatsächliche installieren und benutzen von Verschlüsselung.

* PGP-Email
  * Thunderbird
  * Enigmail
  * evtl GPG4Win (wird von Enigmail automatisch mitinstalliert)
* Android: Wire, Signal, Deltachat

Zum Abschluss: Key-Signing-Party, trust all the fingerprints
