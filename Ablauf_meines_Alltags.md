```mermaid
flowchart TD
    Start["Start"]
    Begruessen["Teamkollegen begrüssen, falls vorhanden"]
    TuerOeffnen["Tür meines Büros öffnen"]
    Auspacken["An meinem Arbeitsplatz<br/>Laptop und Mittagessen aus dem Rucksack auspacken."]
    LaptopCheck["Laptop vorhanden?"]
    TempLaptop["Einen temporären Laptop nehmen<br/>und einloggen"]
    Docking["Laptop an der Docking Station anschliessen"]

    Start --> Begruessen
    Begruessen -- Ja --> Auspacken
    Begruessen -- Nein --> TuerOeffnen
    TuerOeffnen --> Auspacken
    Auspacken --> LaptopCheck
    LaptopCheck -- Ja --> Docking
    LaptopCheck -- Nein --> TempLaptop
    TempLaptop --> Docking