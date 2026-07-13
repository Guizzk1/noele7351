# ZenKernel GKI Builder

Build automatizado do ZenKernel para o Moto G73 5G com Stock ROM.

## Alvo

- Android 12 GKI
- Kernel 5.10 LTS
- Variante normal, com verificação padrão de compatibilidade dos módulos

## Recursos

- [KernelSU Next](https://github.com/pershoot/KernelSU-Next), sempre a partir do HEAD da branch `dev-susfs`
- [SUSFS](https://gitlab.com/simonpunk/susfs4ksu), branch `gki-android12-5.10`

Nenhum patch adicional de rede ou desempenho é aplicado.

## Saída

Cada build publica somente um ZIP flashável no formato:

```text
ZenKernel-<versão-real>-android12-lts-KSUN<versão>-SUSFS<versão>.zip
```

A versão real é lida de `kernel/common/Makefile`, e o resumo registra o
`kernelrelease` compilado, os commits usados e o SHA-256 do ZIP.

## Créditos

- KernelSU Next: pershoot e contribuidores do KernelSU Next
- SUSFS: simonpunk
- AnyKernel3: osm0sis e contribuidores do AnyKernel3

## Aviso

Desbloquear o bootloader e instalar kernels personalizados envolve risco. Faça
backup do boot original e confirme a compatibilidade antes de aplicar o ZIP.
