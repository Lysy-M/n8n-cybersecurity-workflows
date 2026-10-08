# n8n Cybersecurity Workflows

Zanonimizowane przykłady workflow n8n związanych z administracją systemami, monitoringiem, bezpieczeństwem oraz automatyzacją pracy w homelabie.

Repozytorium prezentuje bezpieczne wersje demonstracyjne workflow. Eksporty nie zawierają rzeczywistych poświadczeń, tokenów API, webhooków produkcyjnych ani wewnętrznej adresacji infrastruktury.

Po imporcie wymagają ręcznej konfiguracji własnych credentials, źródeł danych i endpointów.

## Workflow

### `security-alert-triage.json`

Przykładowy proces wstępnej obsługi alertu bezpieczeństwa.

Workflow:

- przyjmuje przykładowy alert,
- normalizuje podstawowe informacje,
- identyfikuje źródło zdarzenia,
- przygotowuje dane do dalszej oceny priorytetu,
- pokazuje sposób organizacji prostego procesu triage.

Przykładowym źródłem zdarzenia jest Wazuh.

Plik:

    workflows/security-alert-triage.json

### `daily-cyber-briefing.json`

Szkielet automatycznego briefingu dotyczącego cyberbezpieczeństwa i infrastruktury.

Zakres przykładowych sekcji:

- krytyczne podatności,
- Linux / Kali / Parrot,
- Wazuh / Suricata,
- Proxmox / Homelab,
- działania do praktycznej weryfikacji w LAB-ie.

Workflow zawiera harmonogram oraz przygotowanie struktury danych, natomiast rzeczywiste feedy i API należy skonfigurować we własnym środowisku.

Plik:

    workflows/daily-cyber-briefing.json

## Import do n8n

1. Otwórz n8n.
2. Wybierz import workflow z pliku.
3. Zaimportuj wybrany plik JSON z katalogu `workflows/`.
4. Skonfiguruj własne credentials i endpointy.
5. Zweryfikuj każdy node przed aktywacją workflow.
6. Przetestuj workflow ręcznie przed uruchomieniem automatycznym.

## Bezpieczeństwo

Repozytorium nie powinno zawierać:

- rzeczywistych credentials,
- tokenów API,
- kluczy webhook,
- kluczy do modeli LLM,
- haseł,
- prywatnych adresów zarządzających,
- pełnych logów zawierających dane osobowe lub informacje wrażliwe.

Dane specyficzne dla środowiska powinny być usuwane lub zastępowane wartościami demonstracyjnymi przed publikacją.

## Zastosowanie w homelabie

n8n wykorzystuję do rozwijania automatyzacji związanej z:

- przetwarzaniem informacji technicznych,
- workflow administracyjnymi,
- analizą i triage zdarzeń bezpieczeństwa,
- przygotowywaniem briefingów,
- integracją różnych usług LAB-u,
- eksperymentami z wykorzystaniem AI w automatyzacji.

Publiczne workflow w tym repozytorium są uproszczonymi i zanonimizowanymi przykładami tych zastosowań.

## Powiązane projekty

- [Cybersecurity & Infrastructure Homelab](https://github.com/Lysy-M/cybersecurity-infrastructure-homelab)
- [Windows Server / Active Directory / VirtualBox Lab](https://github.com/Lysy-M/windows-server-ad-virtualbox-lab)
- [Admin Scripts](https://github.com/Lysy-M/admin-scripts)

## Autor

**Michał Łysiński**

Administrator IT | Linux | Windows Server | Proxmox | Monitoring | Security | Automation
