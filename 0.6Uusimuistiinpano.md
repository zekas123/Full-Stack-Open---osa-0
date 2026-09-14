```mermaid
graph TD;
    html["Käyttäjä vieraili sivulla (HTML, CSS ja JS latautuivat)."] --> print["Käyttäjä kirjoitti tekstin ja napsautti Tallenna-painiketta."];
    print --> js["Selain: lähettää tietoja palvelimelle POST-pyynnön välityksellä."];
    js --> send["Palvelin: tallentaa uuden muistiinpanon ja ohjaa takaisin."];
    send --> server1["Selain: pyytää sivun, CSS:n, JS:n ja datan uudelleen"];
    server1 --> new_save["JS näyttää päivitetyn muistiinpanoluettelon näytöllä, mukaan lukien uuden muistiinpanon"]
    
