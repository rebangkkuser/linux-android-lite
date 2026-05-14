# Projeto Android Linux - Termux

## Descrição

Script de configuração automatizada para instalar e gerenciar um ambiente Linux completo no Termux.

## Recursos

- Detecção automática do dispositivo e GPU
- Suporte a múltiplos ambientes desktop (XFCE4, LXQt, MATE, KDE)
- Aceleração gráfica otimizada por GPU
- Instalação simplificada e automatizada
- Compatibilidade com smartphones e tablets

## Ambientes Desktop Suportados

| Desktop | Peso | Recomendação |
|---------|------|--------------|
| XFCE4   | Médio | Recomendado |
| LXQt    | Leve | Para dispositivos antigos |
| MATE    | Médio | Alternativa estável |
| KDE     | Pesado | Para dispositivos poderosos |

## Instalação

1. Instale o [Termux](https://f-droid.org/pt_BR/packages/com.termux/) do F-Droid
2. Abra o Termux e execute:

```bash
bash script-termux.sh
```

3. Selecione o ambiente desktop desejado
4. Aguarde a instalação ser concluída
5. Rode o script:
```
./start-linux.sh
```
5. Instale o [Termux X11](https://github.com/termux/termux-x11/releases/tag/nightly) para acessar a interface gráfica
6. Abra o Termux X11 e o provedor gráfico já estará funcionando

## Detecção de Hardware

O script detecta automaticamente:
- **Marca do dispositivo**: Samsung, Xiaomi, etc.
- **GPU**: Adreno (Samsung/Qualcomm) ou genérica
- **Driver gráfico**: Freedom ou Zink (compatibilidade)

## Requisitos

- Android 5.0+
- Termux instalado
- Termux: X11
- ~2GB de espaço livre
- Conexão com internet

## Notas

- Use XFCE4 para melhor equilíbrio entre performance e funcionalidade
- Dispositivos antigos: prefira LXQt
- Dispositivos topo de linha: experimente KDE

## Licença

MIT
