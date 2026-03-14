# GitOps structure example

This folder demonstrates a GitOps-friendly repository layout with base and overlays for dev/stage/prod.

Inspired by community best practices for Argo CD / Flux. [web:8][web:11][web:17]

Structure:

- clusters/
  - dev/
  - stg/
  - prod/
- apps/
  - sample-app/
    - base/
    - overlays/
      - dev/
      - stg/
      - prod/
