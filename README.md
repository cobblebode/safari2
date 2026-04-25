# CobbleBode Safari Dungeon Entry v2

Essa versão NÃO cria Hoopa Portal.

O comando:

```mcfunction
/cobblebode dungeon enter <player>
```

faz:
- verifica `cobblesafari:ticket_dungeon`
- remove 1 ticket
- cria uma entrada temporária interna
- chama o `DungeonTeleportHandler` do CobbleSafari
- gera/prepara/teleporta direto para uma dungeon aleatória
- força timer de 30 minutos

## NPC

```mcfunction
/cobblebode dungeon enter @initiator
```

## Build

GitHub Actions já está travado em Gradle 8.10.2.


## v1.0.2

Corrige o erro `Invalid block entity ... Block{minecraft:air}` usando o block state real de `cobblesafari:dungeon_portal` para criar a entrada temporária interna.
