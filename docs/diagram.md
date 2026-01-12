```mermaid
graph TD
    %% Węzły główne
    Start([START])
    Load["Wczytaj Dane<br/>(Oś X: B1, C1... Daty/Kategorie)<br/>(Oś Y: A2, A3... Nazwy/Osoby)"]
    Decision{Czy dane<br/>są poprawne?}
    Error[Wyświetl Błąd]
    Process["Przetwarzanie Danych<br/>(Obliczanie średnich, min/max)"]
    GenView[Generowanie Widoku]
    
    %% Węzły widoków
    Grid["Widok Siatki (Grid)<br/>(Kolorowanie komórek wg wartości)"]
    Chart["Widok Wykresu<br/>(Liniowy lub Słupkowy)"]
    
    %% Węzły końcowe
    Export["Eksport Raportu<br/>(PDF / PNG)"]
    EndNode([KONIEC])

    %% Relacje (Połączenia)
    Start --> Load
    Load --> Decision
    
    Decision -- NIE --> Error
    Decision -- TAK --> Process
    
    Process --> GenView
    
    %% Rozgałęzienie
    GenView --> Grid
    GenView --> Chart
    
    %% Złączenie (Merge)
    Grid --> Export
    Chart --> Export
    
    Export --> EndNode

    %% Stylizacja (Opcjonalna - dla lepszego wyglądu)
    style Start fill:#f9f,stroke:#333,stroke-width:2px
    style EndNode fill:#f9f,stroke:#333,stroke-width:2px
    style Decision fill:#fff5ad,stroke:#d4b600
    style Error fill:#ffb3b3,stroke:#cc0000
    style Export fill:#b3e0ff,stroke:#0066cc