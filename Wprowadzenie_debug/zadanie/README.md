---


# 📝 Zadanie: Postawienie drugiego Gradio z mniejszym Whisperem

Masz już usługę `whisper-gradio` z modelem **Whisper Small**.
Dodaj teraz **drugą usługę**, która uruchamia **Whisper Tiny**.

---

## 1. Zmodyfikuj `app.py`

Dodaj nowy plik, np. `app_tiny.py`, z pipeline dla mniejszego modelu Whisper Tiny.

Uwaga: ustaw port na **8001**, żeby nie kolidował z 8000.

---

## 2. Uruchom serwisy

```bash
docker compose up --build
```

---

## 3. Przetestuj w przeglądarce przez guacamole lub przez forwarding portu

* Whisper Small → [http://localhost:8000](http://localhost:8000)
* Whisper Tiny → [http://localhost:8001](http://localhost:8001)

---

## 4. Test

1. Wgraj ten sam plik audio do obu interfejsów:

   * zmierz czas transkrypcji,
   * porównaj dokładność wyników.

2. W terminalu użyj:

   ```bash
   docker stats
   ```

   Sprawdź:

   * zużycie CPU/RAM przez Whisper Small,
   * zużycie CPU/RAM przez Whisper Tiny.

---

