```mermaid

graph TD
    %% Nagłówek i Użytkownik
    A[APLIKACJA DO ZARZĄDZANIA BUDŻETEM DOMOWYM] --> B(Użytkownik)
    
    %% Główne sekcje aplikacji
    B --> C{Panel główny}
    B --> D[Rejestr wydatków]
    B --> E[Ustawienia]
    
    %% Funkcje Rejestru wydatków
    D --> D1(Dodaj wydatek)
    D --> D2(Edytuj wydatek)
    
    %% Funkcje Ustawień
    E --> E1(Kategoryzacja transakcji)
    E --> E2(Budżet miesięczny + progi)
    E --> E3(Powiadomienia o przekroczeniu)
    
    %% Wspólny element wynikowy / wizualizacja
    E1 --> F{Wizualizacja wydatków - Wykresy, statystyki}
    E2 --> F
    E3 --> F
    
    %% Styling dla lepszej czytelności (opcjonalnie)
    classDef mainSection fill:#f9f,stroke:#333,stroke-width:2px;
    class C,D,E mainSection;
    class A,B,F default;
