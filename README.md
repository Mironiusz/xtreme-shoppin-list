# Shoppin' List 2000

## Opis projektu
Shoppin' List 2000 to aplikacja webowa stworzona w Vue 3, która pomaga użytkownikom zarządzać listami zakupowymi. Pozwala na dodawanie, edytowanie i udostępnianie list zakupowych innym użytkownikom. Aplikacja wykorzystuje REST API do przechowywania danych na serwerze.

## Technologie
Projekt został zbudowany przy użyciu następujących technologii:
- **Vue 3** - framework frontendowy
- **Vue Router** - zarządzanie trasami
- **Vue Toastification** - powiadomienia
- **Axios** - komunikacja z API
- **SCSS** - stylizacja komponentów
- **Three.js** - grafika 3D (efekty wizualne w tle)

## Funkcjonalności
✅ Tworzenie i edycja list zakupowych
✅ Oznaczanie elementów jako kupione
✅ Współdzielenie listy z innymi użytkownikami
✅ Automatyczne logowanie i sesje użytkownika
✅ Powiadomienia o akcjach użytkownika
✅ Synchronizacja z API
✅ Efekty wizualne 3D z wykorzystaniem Three.js

## Instalacja i uruchomienie
1. **Klonowanie repozytorium:**
   ```sh
   git clone https://github.com/NAZWA_UŻYTKOWNIKA/NAZWA_REPO.git
   cd NAZWA_REPO
   ```

2. **Instalacja zależności:**
   ```sh
   npm install
   ```

3. **Uruchomienie aplikacji:**
   ```sh
   npm run dev
   ```
   Aplikacja będzie dostępna pod adresem `http://localhost:5173/`

## Struktura projektu
```
📂 src/
├── 📂 components/  # Komponenty wielokrotnego użytku (przyciski, formularze, inputy itp.)
├── 📂 models/      # Modele danych (Listy, Przedmioty)
├── 📂 views/       # Widoki stron aplikacji
├── 📂 router/      # Konfiguracja tras
├── 📂 assets/      # Zasoby (obrazy, ikony itp.)
└── main.js        # Główny plik aplikacji
```

## API
Aplikacja komunikuje się z backendem poprzez REST API. Oto kilka kluczowych endpointów:
- `GET /api/lists/getAllLists` - pobranie wszystkich list użytkownika
- `POST /api/lists/addNewList` - dodanie nowej listy
- `PUT /api/lists/renameList/{id}` - zmiana nazwy listy
- `DELETE /api/lists/deleteListById/{id}` - usunięcie listy
- `POST /api/auth/login` - logowanie użytkownika
- `POST /api/auth/register` - rejestracja użytkownika
