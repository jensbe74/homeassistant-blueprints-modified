# Home Assistant Blueprint Modifications

This repository contains modified Home Assistant blueprints.

**Original Repository:** [panhans/HomeAssistant](https://github.com/panhans/HomeAssistant)
**License:** [MIT License](https://github.com/panhans/HomeAssistant/blob/main/LICENSE)

## 🔥 Advanced Heating Control JB -V5

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

#### Dateien in diesem Repository:
- [advanced_heating_control_jb_v5.yaml](blueprints/advanced_heating_control_jb_v5.yaml)
- [advanced_heating_control_sensor_jb.yaml](blueprints/advanced_heating_control_sensor_jb.yaml)
- [scene_toggle_jb.yaml](blueprints/scene_toggle_jb.yaml)
