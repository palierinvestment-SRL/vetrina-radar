# Vetrina Radar

Pagina pubblica del Radar trend: accesso con Google, nessun dato utente salvato.

- `index.html`: interfaccia (Google Identity Services, dati solo in sessionStorage)
- `privacy.html`: informativa
- Server: Supabase Edge Function `radar-public` (verifica il token Google a ogni richiesta)
- Motore orario: Supabase Edge Function `radar-fetch` + pg_cron (Google Trends RSS Italia, YouTube Data API v3)
