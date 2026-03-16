APBD - Ćwiczenia 2 - Pytania

Pytanie 1:
Kiedy Git wykonuje fast-forward, a kiedy powstaje merge commit?

Fast-forward powstaje gdy gałąź docelowa nie ma żadnych nowych commitów od momentu utworzenia gałęzi funkcjonalnej.
Za to merge commit powstaje, gdy obie gałęzie zawierają nowe commity.

Pytanie 2:
Czym w praktyce różni się merge od rebase?

Merge zachowuje historię rozgałęzień i tworzy merge commit, pokazując, że prace były równoległe.
Za to rebase przepisuje historię gałęzi, umieszczając jej commity na końcu innej gałęzi, tworząc liniową historię bez merge commitów.

Pytanie 3:
W jaki sposób został rozwiązany konflikt w repozytorium?

Konflikt powstał, gdy ta sama linia w Program.cs była zmieniona w gałęzi feature-conflict i w main.
Rozwiązałam go ręcznie w następujący sposób:

1. Otworzyłam plik i usunęłam markery konfliktu (Znaki takie jak: <<<<<<<, =======, czy >>>>>>>)

2. Połączyłam obie zmiany w jedną sensowną linię, tak aby program dalej działał poprawnie.

3. Następnie dodałam zmieniony plik (git add) i zakończyłam merge (git commit).
