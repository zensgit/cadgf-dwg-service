# cadgf-dwg-service

DWG conversion service for CADGameFusion, built around LibreDWG for SaaS deployments.

## Scope
- Accept DWG uploads and convert them to formats CADGameFusion can ingest (DXF/JSON/GLTF).
- Keep the conversion component isolated so core CADGameFusion stays license-clean.

## Planned API (draft)
- `POST /convert` (multipart form-data): `file=@drawing.dwg`
- Response includes paths/URLs to converted artifacts.

## Licensing
- GPL-3.0 (matches LibreDWG).
- Intended for server-side (SaaS) deployments. Distributing binaries to customers requires GPL compliance.

## Status
- Repository scaffold only. Implementation pending.
