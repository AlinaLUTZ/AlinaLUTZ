# 🛡️ Инженер ИБ-ориентированной суверенной ИИ-автоматизации

> ⚠️ **Демонстрационный профиль. Все права защищены.**  
> Материалы опубликованы исключительно в целях профессионального портфолио.  
> Любое использование, копирование или внедрение без письменного разрешения автора запрещено.  
> Коммерческое применение, аудит и интеграция доступны по договору.

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
🧠 [Исследовательские направления](RESEARCH.md)  
🧮 [Прикладная математика](MATH_CHECKLIST.md)

Проектирую **архитектуру ИИ-систем с принципом «безопасность от проектирования» (Security by Design)** для юридических и земельных процессов в Российской Федерации.  
Мои решения **не обрабатывают персональные данные**, размещаются **исключительно на инфраструктуре в РФ** и **готовы к ИБ-аудиту** в соответствии с требованиями регуляторов.

Этот репозиторий — часть систематизации моей экспертизы. Здесь я публикую **шаблоны, методики и архитектурные паттерны** для суверенных, аудитуемых и compliance-ready ИИ-автоматизаций.

---

## 📌 Доступные шаблоны и инструменты

- [**secure-land-contract-parser**](https://github.com/AlinaLUTZ/secure-land-contract-parser) — offline-парсер для полного обезличивания договоров аренды земли по ФЗ-152. Zero PII, без интернета, готов к ИБ-аудиту.  
- [Системный промт для наставника по безопасной ИИ-экспертизе](prompts/mentor_secure_vibecoder.md)  
- [Генератор compliance-описания для ИИ-автоматизаций](prompts/compliance_description_generator.md)  
- [Анализ ВРИ (видов разрешённого использования) без ПДн](prompts/land_vri_analyzer.md)  
- [Анализ договора аренды земельного участка (без ПДн)](prompts/land_lease_contract_analyzer.md)  
- [Чек-лист подачи заявления на землю для КФХ (без ПДн)](prompts/kfh_land_application_checklist.md)  
- [Генератор официального запроса в администрацию (без ПДн)](prompts/admin_request_generator.md)

---

## 🔧 Архитектурный стек: безопасность как основа

Все решения проектируются в соответствии с принципом **«Security by Design»**: безопасность закладывается на этапе архитектуры, а не добавляется как надстройка.

### 🛠️ Среда разработки и развёртывания
- **Cursor AI** — локально ориентированный ИИ-ассистент, не передающий исходный код во внешние API  
- **Docker + Docker Compose** — изоляция компонентов, воспроизводимость окружения, контроль зависимостей  
- **Self-hosted VPS (РФ)** — развёртывание исключительно на инфраструктуре в Российской Федерации с полным контролем над данными и доступом  

### 🔄 Оркестрация и автоматизация
- **n8n (self-hosted)** — low-code платформа оркестрации с поддержкой RBAC, TLS-шифрования и аудит-логов  
- **PostgreSQL** — реляционная СУБД с row-level security и возможностью дополнительного шифрования данных на уровне приложения  

### 🤖 Генеративные модели (адаптированные под ИБ и суверенитет)

Выбор модели диктуется задачей, но **любое использование строго ограничено** безопасным, аудитуемым и законным режимом. Все модели запускаются локально или в изолированной среде — **без передачи данных во внешние сервисы**.

#### ⚙️ Используемые модели (без обработки ПДн)
- **Юридический анализ**: LLaMA 3 70B, Mistral Large, Qwen-Max, DeepSeek-Law  
- **Генерация кода**: Code Llama, StarCoder2, DeepSeek-Coder  
- **Мультимодальный анализ**: LLaVA-NeXT, Qwen-VL (применяются только к публичным, неперсонализированным скан-образам)  

### 🛡️ Инструменты информационной безопасности (в активной интеграции)
- **Моделирование угроз**: LINDDUN (специализированный для ИИ-систем), STRIDE  
- **Управление секретами**: HashiCorp Vault  
- **Аудит и мониторинг**: Loki + Grafana, auditd  
- **Сканирование уязвимостей**: Trivy (для Docker-образов), Clair  
- **Защита данных и инфраструктуры**:  
  - TLS-терминация через Traefik  
  - Шифрование дисков (LUKS)  
  - Сегментация сети на уровне хоста и контейнеров  

---

## 🎯 Для кого это
- **Госсектор**: Минэкономразвития, Росреестр, региональные АИЖК  
- **Финансовые институты**: Россельхозбанк и другие организации с государственным участием  
- **Юридические и земельные компании**, работающие в условиях строгого регулирования

---

## 💡 Основа решений

Проектирую **ИБ-зрелые ИИ-процессы**, которые можно внедрять **без риска остановки на compliance-проверке, штрафов или утечек** — потому что безопасность заложена в архитектуру, а не добавлена сверху.

---

## 📄 Правовая и ИБ-информация
- **Авторские права**: см. [`LICENSE`](./LICENSE) — все права защищены  
- **Политика информационной безопасности**: см. [`SECURITY.md`](./SECURITY.md)

📬 **Открыта к коллаборациям** в сфере суверенного ИИ для земельных, правовых и государственных процессов.

---

🕗 Последнее обновление: 27 декабря 2025 г.
