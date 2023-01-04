# 4IT575 SW Architektury
Repozitář pro seminární práci pro předmět 4IT575 Softwarové Architektury

## Obsah
- [Zadání aplikace] (https://github.com/rronaldr/4IT575-Architektury#zad%C3%A1n%C3%AD-aplikace)
- [Popis 1. architektury (microservices)] (https://github.com/rronaldr/4IT575-Architektury/tree/main/Microservices/ADR/1-microservices-decision#microservice-adr)
- [Popis 2. architektury] (https://github.com/rronaldr/4IT575-Architektury/tree/main/EDA#dokumentace-2-architektury)

## Zadání aplikace
**Popis aplikace:**

Prodejní portál vstupenek na koncerty s velkými počty akcí a velkým objemem vstupenek potřebuje pro svou činnost pružné řešení.
Uživatelé: tisíce souběžných uživatelů, nárazy až 10 000 uživatelů za sekundu při prodeji vstupenek.

**Požadavky:**
- umožnit souběžný nákup vstupenek
- neprodat žádné místo více než jednou!
- nakupující vidí přehled zbývajících míst

## Zvolené architektury
- Microservices
    - ADR o rozhodnutí
- Event driven architecture
    - ADR o rozhodnutí

### Autoři
Jan Hála, Pavel Dohnal, Martin Macko, Ronald Rebernigg
