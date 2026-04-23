# Home Assistant Blueprint Modifications

This repository contains modified Home Assistant blueprints.

**Original Repository:** [panhans/HomeAssistant](https://github.com/panhans/HomeAssistant)
**License:** [MIT License](https://github.com/panhans/HomeAssistant/blob/main/LICENSE)

## 🔥 Advanced Heating Control (Modified)

### Änderungen am 23.04.2026

Der Blueprint wurde erweitert, um zusätzliche Anwesenheitsentitäten zu unterstützen.

#### Neue Funktionen:
- **Zusätzliches Eingabefeld:** `input_person_entities` (👥 Additional Presence Entities) hinzugefügt.
- **Erweiterte Domänen-Unterstützung:** Es können nun mehrere Entitäten aus den Domänen `binary_sensor`, `input_boolean`, `sensor` und `switch` ausgewählt werden.
- **Logik-Erweiterung:**
    - Der Status `on` dieser Entitäten wird nun als Anwesenheit ("home") gewertet.
    - Vollständige Integration in die `is_anybody_home` Logik, inklusive Berücksichtigung der Verzögerungszeiten für Kommen und Gehen.
    - Integration in die Frostschutz-Logik (`is_frost_protection`).
    - Korrekte Behandlung in der `is_minimal_config` Prüfung.

#### Datei:
- [advanced_heating_control.yaml](file:///C:/Antigravity-Projekte/homeassistant/blueprints/automation/panhans/advanced_heating_control.yaml)
