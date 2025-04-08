![Postman](https://img.shields.io/badge/Postman-10%2B-orange)
![License](https://img.shields.io/badge/License-MIT-purple)
![Tested APIs](https://img.shields.io/badge/Tested%20APIs-Reqres%20%26%20PokeAPI-blueviolet)


[➡️ Click here to open the Postman workspace](https://www.postman.com/whiskeyprincess/workspace/portfolio-paulina)
[🇬🇧 English](#-english-version) | [🇵🇱 Polski](#-wersja-polska)

---
## 🇬🇧 English version
# 🧪 Postman Tests – API Automation Suite

This workspace contains three Postman collections created as part of a portfolio project.  
The main goal was to demonstrate skills in testing REST APIs using Postman, JavaScript, and schema validation.  

---

## ✅ Test Coverage

- HTTP methods: `GET`, `POST`, `PUT`, `PATCH`, `DELETE`
- JSON Schema validation
- Saving values to collection variables
- Token handling and authorization
- Negative testing (invalid login, empty fields)
- Visualizer with dynamic HTML summary
- Response validation: status, content, structure
- Use of public APIs: Reqres, PokeAPI

---

## 📁 Collections included

| Collection | Description |
|-----------|-------------|
| **PokeApi** | Basic GET testing of Pokémon data from the public API |
| **PokeApi – Pokemon Battle** | Comparing two Pokémon stats and displaying a winner using visualizer |
| **ReqresApi** | Full CRUD and login/register testing with token, schemas, edge cases |

---

## 📂 Project Structure

```text
Portfolio Paulina (Postman Workspace)
├── PokeApi
│   └── Pokemon
├── PokeApi - pokemon battle
└── ReqresApi
    ├── Users
    ├── Authentication
    └── Resources

--- 

## 🧪 Example Test – ensure uniqueness of language names and urls in genera

```JavaScript
  const response = pm.response.json()
  pm.test("ensure uniqueness of language names and urls in genera", () => {
    const name = response.genera.map(name => name.language.name)
    const uniqueName = new Set(name)
    pm.expect(name.length).is.equal(uniqueName.size)
    const url = response.genera.map(url => url.language.url)
    const uniqueUrl = new Set(url)
    pm.expect(url.length).is.equal(uniqueUrl.size)
})
```

## 📸 Preview

![image](https://github.com/user-attachments/assets/a271586e-4c4a-4a0e-8815-1f57b7c122ee)

--- 

## 🧰 Tech Stack

- **Postman** – test case management, request building, assertions, Collection Runner
- **JavaScript (Chai)** – assertions, logic control inside tests
- **JSON Schema** – validation of API response structures
- **Postman Collection Variables** – storing and reusing dynamic values across requests
- **Pre-request scripts** – generating data before execution
- **HTML Visualizer** – rendering test results in dynamic HTML (used in Pokémon Battle)
- **Public REST APIs**:
  - [Reqres](https://reqres.in)
  - [PokeAPI](https://pokeapi.co)

---

## ▶️ How to use

The easiest way is to open the public Postman workspace:

➡️ [Click here to view the workspace](https://www.postman.com/whiskeyprincess/workspace/portfolio-paulina)

---

## 🎯 What I Learned

- Structuring and organizing collections for real-world projects
- Writing reusable and clear tests in Postman
- Using variables and pre-request scripts to make requests dynamic
- Creating visual summaries using the Visualizer feature
- Validating API responses against JSON schemas
- Handling edge cases and writing negative tests

---

## 👩‍💻 Author 🩷
Project created by Paulina Wróblewska. 💖  
🔗 [GitHub](https://github.com/Paulina-Wroblewska)

🔗 [LinkedIn](https://www.linkedin.com/in/paulina-wr%C3%B3blewska-2381a217b/)



[➡️ Kliknij tutaj, aby przejść do workspace'a w Postmanie](https://www.postman.com/whiskeyprincess/workspace/portfolio-paulina)  

---
## 🇵🇱 Wersja polska
# 🧪 Testy API w Postmanie – Zestaw Kolekcji

Ten workspace zawiera trzy kolekcje stworzone w Postmanie jako część projektu do portfolio.  
Celem było zaprezentowanie umiejętności testowania REST API z użyciem Postmana, JavaScriptu oraz walidacji odpowiedzi.

---

## ✅ Zakres testów

- Metody HTTP: `GET`, `POST`, `PUT`, `PATCH`, `DELETE`
- Walidacja schematów odpowiedzi (JSON Schema)
- Zapis danych do zmiennych kolekcji
- Obsługa tokenów i autoryzacja
- Testy negatywne (błędne logowanie, brak danych)
- Wizualizacja wyników w formacie HTML
- Walidacja odpowiedzi: status, struktura, zawartość
- Użycie publicznych API: Reqres, PokeAPI

---

## 📁 Zawarte kolekcje

| Kolekcja | Opis |
|----------|------|
| **PokeApi** | Podstawowe testy `GET` na danych Pokémon z publicznego API |
| **PokeApi – Pokemon Battle** | Porównanie statystyk dwóch Pokémonów i wyświetlenie zwycięzcy |
| **ReqresApi** | Pełne testowanie CRUD + logowanie/rejestracja, tokeny, walidacja schematów i przypadki brzegowe |

---

## 📂 Struktura projektu

```text
Portfolio Paulina (Postman Workspace)
├── PokeApi
│   └── Pokemon
├── PokeApi - pokemon battle
└── ReqresApi
    ├── Users
    ├── Authentication
    └── Resources
```

---
## 🧪 Przykładowy test – sprawdzenie unikalności nazw języków i URL w genera

```JavaScript
  const response = pm.response.json()
  pm.test("ensure uniqueness of language names and urls in genera", () => {
    const name = response.genera.map(name => name.language.name)
    const uniqueName = new Set(name)
    pm.expect(name.length).is.equal(uniqueName.size)
    const url = response.genera.map(url => url.language.url)
    const uniqueUrl = new Set(url)
    pm.expect(url.length).is.equal(uniqueUrl.size)
})
```

## 📸 Podgląd

Poniżej znajduje się przykładowy zrzut ekranu pokazujący wizualizację

![image](https://github.com/user-attachments/assets/a271586e-4c4a-4a0e-8815-1f57b7c122ee)

--- 

## 🧰 Stack technologiczny

- **Postman** – przygotowanie requestów, tworzenie testów, Collection Runner
- **JavaScript (Chai)** – logika i warunki testowe
- **JSON Schema** – walidacja struktury odpowiedzi
- **Zmienne kolekcji** – dynamiczne przechowywanie danych
- **Skrypty pre-request** – generowanie danych przed wykonaniem testów
- **HTML Visualizer** – wizualne podsumowanie testów (np. w Pokémon Battle)
- **Publiczne REST API**:
  - [Reqres](https://reqres.in)
  - [PokeAPI](https://pokeapi.co)

---

## ▶️ Jak korzystać z projektu
Najprostszy sposób to otwarcie workspace’a:

➡️ [Kliknij tutaj, aby przejść do workspace'a](https://www.postman.com/whiskeyprincess/workspace/portfolio-paulina)

--- 

## 🎯 Czego się nauczyłam

- Organizowania i strukturyzowania kolekcji w realnych projektach
- Pisania czytelnych i wielokrotnego użytku testów w Postmanie
- Użycia zmiennych i pre-requestów do dynamicznych danych
- Tworzenia podsumowań HTML z wykorzystaniem Visualizera
- Walidacji odpowiedzi przy pomocy JSON Schema
- Obsługi błędów, testowania negatywnych scenariuszy

---

## 👩‍💻 Autor 🩷
Projekt stworzony przez **Paulinę Wróblewską** 💖  
🔗 [GitHub](https://github.com/Paulina-Wroblewska)

🔗 [LinkedIn](https://www.linkedin.com/in/paulina-wr%C3%B3blewska-2381a217b/)
