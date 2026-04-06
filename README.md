# LAMP Deployment with Ansible

Ten projekt automatyzuje instalację stosu LAMP na systemach z rodziny Debian/Ubuntu.

## Struktura Ról
* **base**: Przygotowanie systemu (aktualizacja, narzędzia pomocnicze).
* **database**: Instalacja MariaDB, konfiguracja bazy `lamp_db`.
* **web**: Instalacja serwera Apache2.
* **php**: Instalacja interpretera PHP i integracja z serwerem WWW.
* **app**: Wdrożenie testowej strony PHP weryfikującej połączenie z MySQL.

## Dostosowanie
Możesz zmienić dane logowania do bazy danych w pliku `roles/database/defaults/main.yml`.

## Użycie
1. Upewnij się, że masz zainstalowane Ansible oraz dostęp SSH do serwera.
2. Edytuj plik `inventory.ini`, wpisując adres IP serwera docelowego.
3. Uruchom playbook komendą:
   ```bash
   ansible-playbook -i inventory.ini site.yml# Zadanie_18_learnIT
