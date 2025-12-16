# Taller 5 — Ansible Vault y recuperación de contraseña (entrega del alumno)

Objetivo
- Usar Ansible Vault para almacenar variables sensibles y demostrar cómo recuperar/usar la contraseña de vault sin subir secretos al repo.

Archivos esperados
- `taller5/host.ini`
- `taller5/playbook_vault.yml` que use variables cifradas con `ansible-vault`.
- `taller5/vault` (archivo cifrado) o `group_vars/` cifrados.
- `taller5/README.md` — este archivo, con explicación clara de cómo se obtuvo el password o cómo se usó `--vault-password-file`.

Notas importantes
- No subir passwords en texto plano.
- Si el enunciado del curso facilita un playbook `retrieve_vault_password.yml`, explicar en README cómo se integró (o cómo se suministró la contraseña en clase).

Validaciones
- `ansible-vault view` local (no en el repo) para comprobar el contenido cifrado.
- Ejecución del playbook con `--ask-vault-pass` o `--vault-password-file` según tu método.

Entregable
- Playbook que use variables cifradas, inventario y README con pasos para ejecutar y evidencia.
