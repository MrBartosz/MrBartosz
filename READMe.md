# Bartosz Maksimowski

Frontend Developer → Automatyk w Kuchnia Vikinga.  
Wykonuję obowiązki automatyka + tworzę software, który rozwiązuje realne problemy na hali produkcyjnej.

---

## SERWISO — CMMS/EAM SaaS

> [serwiso.vercel.app](https://serwiso.vercel.app/login)

System zarządzania utrzymaniem ruchu i serwisem maszyn. Wdrożony w środowisku produkcyjnym — 60+ maszyn, praca ciągła 24/7.

### Co robi

- **Zlecenia serwisowe** — pełny lifecycle (open → in_progress → approval → done), przypisania, komentarze
- **Zgłaszanie awarii** — operator zgłasza usterkę maszyny → tworzy się zlecenie → technik widzi je na liście i idzie naprawić
- **Zarządzanie maszynami** — QR code do każdej maszyny, mapa hali (drag & drop), motogodziny, koszt przestoju PLN/h
- **Magazyn części** — stany, alerty low-stock, wydania na zlecenie, kompatybilność maszyna ↔ część
- **Kalendarz** — widok miesięczny z filtrami (maszyna, przypisany, status), tworzenie i edycja zdarzeń
- **Harmonogram zmian** — silnik generujący automatyczny grafik 24/7 (4/5-brygadowy)
- **Konserwacja** — harmonogramy przeglądów (czas / motogodziny / hybrid), automatyczne generowanie zadań
- **Digital Twin 3D** — interaktywny model maszyny (cyfrowy bliźniak) — _aktualnie w trakcie rozwoju_
- **Tryb kiosku** — wspólny tablet na hali, logowanie PIN-em, szybkie przełączanie profili
- **AI Copilot** — techniczny chatbot, który doradza przy problemach z maszynami
- **Import danych** — bulk import maszyn, części i zleceń z CSV/Excel
- **Tryb gościa** — read-only wersja aplikacji dla osób, które chcą ją przejrzeć bez rejestracji

### Stack

| Warstwa | Technologia |
|---------|-------------|
| Frontend | Next.js 14, React 18, TypeScript, Tailwind, Framer Motion, Recharts, Three.js |
| Backend | NestJS, Prisma (62 modele), Zod, Passport-JWT, BullMQ (13 procesorów) |
| Baza | PostgreSQL 16 (Neon) + pgvector |
| Cache/Queues | Redis 7 (Upstash) |
| AI | OpenAI GPT-4o-mini + ada-002 embeddings, circuit breaker |
| Auth | JWT + 2FA/TOTP + Magic Link + PIN/Kiosk + SSO (Azure/Google/Okta) |
| Infra | Vercel (frontend), Railway/Render (backend Docker), OpenTelemetry, Sentry |
| CI | GitHub Actions, Husky, Turborepo, Playwright E2E, Stryker mutation testing |
| i18n | 4 języki (PL, EN, DE, UA) |

---

## Kontakt

✉️ [maksimowski97@gmail.com](mailto:maksimowski97@gmail.com)
