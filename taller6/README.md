# Taller 6 — Pruebas automáticas (Molecule) y CI (entrega del alumno)

Objetivo
- Añadir pruebas automáticas para un role (Molecule + testinfra/pytest) y demostrar idempotencia y lint en CI.

Archivos esperados
- `taller6/host.ini` (si aplica) o configuración `molecule/` para driver (docker, instance).
- `taller6/roles/<role>/` con `molecule/default/molecule.yml` y `molecule/default/tests/test_default.py` (testinfra).
- `taller6/verify.sh` (script que ejecuta checks básicos: curl, systemctl, etc.).
- Opcional: un workflow en `.github/workflows/` que ejecute `ansible-lint` y `molecule test`.
- `taller6/README.md` — este archivo.

Validaciones mínimas
- `molecule test` (o `molecule converge` + `molecule verify`)
- `ansible-lint` y `ansible-playbook --syntax-check`
- Demostrar idempotencia: segunda ejecución sin cambios.

Entregable
- Role con Molecule y tests, script de verificación e instrucciones en README con salidas de pruebas.
