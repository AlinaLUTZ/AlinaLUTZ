# 🛡️ Инженер ИБ-ориентированной суверенной ИИ-автоматизации

<!-- Compliance & Domain -->
![Land Tech](https://img.shields.io/badge/Land_Tech-Specialist-lightgrey?logo=mapbox&labelColor=3a3a3a)
![ФЗ-152](https://img.shields.io/badge/ФЗ--152-Compliant-green?logo=russia&labelColor=0039a6)
![Sovereign AI](https://img.shields.io/badge/Sovereign_AI-Yes-blue?logo=linux&labelColor=000000)
![Zero PII](https://img.shields.io/badge/Zero_PII-✓-red?logo=privacy&labelColor=8b0000)
![Self-Hosted](https://img.shields.io/badge/Self--Hosted-in_RU-orange?logo=github&labelColor=444444)

<!-- AI & Models -->
![Cursor](https://img.shields.io/badge/Cursor-Local_AI_Assistant-black?logo=cursor&logoColor=white)
![Replit](https://img.shields.io/badge/Replit-Offline_Mode-purple?logo=replit&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-Local_Editor-blue?logo=visual-studio-code&logoColor=white)

<!-- Infrastructure -->
![n8n](https://img.shields.io/badge/n8n-Self--Hosted-blue?logo=n8n&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-RLS_Enabled-336791?logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Isolated-orange?logo=docker&logoColor=white)
![Vault](https://img.shields.io/badge/HashiCorp_Vault-Secrets_Management-ff0033?logo=hashicorp&logoColor=white)

<!-- Security Tooling -->
![Bandit](https://img.shields.io/badge/Bandit-SAST-green?logo=python&logoColor=white)
![Semgrep](https://img.shields.io/badge/Semgrep-Code_Scanning-2b0066?logo=semgrep&logoColor=white)

📚 [Профессиональные компетенции](SKILLS.md)  
🧠 [Мои исследовательские направления](RESEARCH.md) 

🧮 [Прикладная математика](MATH_CHECKLIST.md)

Проектирую **архитектуру AI-систем с «безопасностью от проектирования» (Security by Design)** для юридических и земельных процессов в Российской Федерации.  
Мои решения исключают обработку ПДн, размещаются на инфраструктуре в РФ и пригодны к ИБ-аудиту по требованиям регуляторов.

Этот репозиторий — часть систематизации моей экспертизы. Здесь я публикую шаблоны, методики и архитектурные паттерны для суверенных, аудитуемых и compliance-ready AI-автоматизаций.

📌 Доступные шаблоны и инструменты:

- [**secure-land-contract-parser**](https://github.com/AlinaLUTZ/secure-land-contract-parser) — offline-парсер для полного обезличивания договоров аренды земли по ФЗ-152. Zero PII, без интернета, готов к ИБ-аудиту.
- [Системный промт для наставника по безопасному AI-экспертизу](prompts/mentor_secure_vibecoder.md)  
- [Генератор compliance-описания для ИИ-автоматизаций](prompts/compliance_description_generator.md)  
- [Анализ ВРИ (видов разрешённого использования) без ПДн](prompts/land_vri_analyzer.md)  
- [Анализ договора аренды земельного участка (без ПДн)](prompts/land_lease_contract_analyzer.md)  
- [Чек-лист подачи заявления на землю для КФХ (без ПДн)](prompts/kfh_land_application_checklist.md)  
- [Генератор официального запроса в администрацию (без ПДн)](prompts/admin_request_generator.md)
  



---

## 🔧 Архитектурный стек: безопасность как основа

Я строю решения на основе следующих принципов и технологий:

### 🛠️ Среда разработки и развёртывания
- **Cursor AI** — локально-ориентированный ИИ-ассистент (без отправки кода во внешние API)  
- **Docker + Docker Compose** — изоляция компонентов, воспроизводимость, контроль зависимостей  
- **Self-hosted VPS (РФ)** — полный контроль над данными и инфраструктурой

### 🔄 Оркестрация и автоматизация
- **n8n (self-hosted)** — low-code оркестрация с поддержкой RBAC, TLS и аудит-логов  
- **PostgreSQL** — СУБД с поддержкой row-level security и шифрования на стороне приложения

### 🤖 Генеративные модели (адаптированные под ИБ и суверенитет)

Мои решения строятся на принципе: **«Использую ту модель, которая решает задачу — но только в безопасном, аудитуемом и законном режиме»**.

#### ⚙️ Дополнительные модели ( без ПДн)
- **Юридический анализ**: LLaMA 3 70B, Mistral Large, Qwen-Max, DeepSeek-Law  
- **Генерация кода**: Code Llama, StarCoder2, DeepSeek-Coder  
- **Мультимодальность**: LLaVA-NeXT, Qwen-VL (только для публичных сканов)

### 🛡️ Инструменты информационной безопасности (в активной интеграации)
- **Анализ угроз**: LINDDUN для ИИ-систем, STRIDE-моделирование  
- **Управление секретами**: HashiCorp Vault  
- **Аудит и мониторинг**: Loki + Grafana, auditd  
- **Сканирование уязвимостей**: Trivy (для Docker-образов), Clair  
- **Защита данных**: TLS через Traefik, шифрование дисков (LUKS), network segmentation

---

## 🎯 Для кого это
- **Госсектор**: Минэкономразвития, Росреестр, региональные АИЖК  
- **Финансовые институты**: Россельхозбанк и другие с госучастием  
- **Юридические и земельные компании**, работающие в условиях строгого регулирования

---

## 💡 Основа решений 
Проектирую **ИБ-зрелые AI-процессы**, которые можно внедрять **без риска остановки на compliance-проверке, штрафов или утечек** — потому что безопасность заложена в архитектуру, а не добавлена поверх.

---

📬 **Открыта к коллаборациям** в сфере суверенного ИИ для земли, права и госпроцессов.  
🔗 Политика информационной безопасности — см. [`SECURITY.md`](SECURITY.md)

---
🕗 Последнее обновление: 24 декабря 2025
