```mermaid
flowchart TD
    Start["Start"]
    Begruessen["Teamkollegen begrüssen, falls vorhanden"]
    TuerOeffnen["Tür meines Büros öffnen"]
    Auspacken["An meinem Arbeitsplatz<br/>Laptop und Mittagessen aus dem Rucksack auspacken."]
    LaptopCheck["Laptop vorhanden?"]
    TempLaptop["Einen temporären Laptop nehmen<br/>und einloggen"]
    Docking["Laptop an der Docking Station anschliessen"]
    Mittagessen["Mittagessen vorhanden?"]
    Küche1["Zur Küche gehen"]
    Kühlschrank["Zur Küche gehen und<br/>es im Hühlschrank<br/>rein tun"]
    Glas1["Ist ein Glas vorhanden?"]
    Glas2["Glas nehmen"]
    Tasse1["Ist eine Tasse vorhanden"]
    Spühlmaschine["Spühlmaschine<br/>schauen und ein<br/>Glas/Tasse nehmen<br/>oder eins sauber machen"]
    Glas/Tasse["Glas/Tasse mit<br/>Wasser auffüllen"]
    WegBüro["Zurück ins Büro gehen"]
    LTstart["Schauen, ob mein Laptop gestartet hat"]
    LTon["Laptop einschalten"]
    LTapp["Einloggen und Teams, Outlook, OneNote und den Ticketsystem starten"]
    Nachrichten["Mails durch schauen und danach schaue ich meine Teams Nachrichten an"]
    Ticket1["Gibt es Ticket udpates?"]
    Ticket2["Nächsten schritt schauen für den Ticket"]
    UnassignedTicket["Gibt es Unassigned Tickets?"]
    Ticket5["Ticket nehmen"]
    Queue["Meine Tickets bearbeiten"]
    Ende["Ende"]

    Start --> Begruessen
    Begruessen -- Ja --> Auspacken
    Begruessen -- Nein --> TuerOeffnen
    TuerOeffnen --> Auspacken
    Auspacken --> LaptopCheck
    LaptopCheck -- Ja --> Docking
    LaptopCheck -- Nein --> TempLaptop
    TempLaptop --> Docking
    Docking --> Mittagessen
    Mittagessen -- Ja --> Kühlschrank
    Mittagessen -- Nein --> Küche1
    Küche1 --> Glas1
    Kühlschrank --> Glas1
    Glas1 -- Ja --> Glas2
    Glas1 -- Nein --> Tasse1
    Glas2 --> Glas/Tasse
    Tasse1 -- Ja --> Glas/Tasse
    Tasse1 -- Nein --> Spühlmaschine
    Spühlmaschine --> Glas/Tasse
    Glas/Tasse --> WegBüro
    WegBüro --> LTstart
    LTstart -- Ja --> LTapp
    LTstart -- Nein --> LTon
    LTon --> LTapp
    LTapp --> Nachrichten
    Nachrichten --> Ticket1
    Ticket1 -- Ja --> Ticket2
    Ticket1 -- Nein --> UnassignedTicket
    Ticket2 --> UnassignedTicket
    UnassignedTicket -- Ja --> Ticket5
    Ticket5 --> Queue
    UnassignedTicket -- Nein --> Queue
    Queue --> Ende