# VXM Database Backups

Respaldos automáticos diarios de la base de datos de VentasVXM.

**Último backup:** se actualiza automáticamente cada día a las 9:00 PM (Guatemala).

## Restaurar un backup

```bash
gunzip -c backup_YYYY-MM-DD_HHMM.sql.gz | psql "postgresql://postgres:[PASSWORD]@db.fuyqhcswcluvozkfluwg.supabase.co:5432/postgres"
```

## Contenido

Solo incluye el schema `public` (tablas de la app). No incluye schemas internos de Supabase (auth, storage, realtime, etc.).
