# BlockSlayer

[中文](#中文) · [English](#english) · [Español](#español)

## 中文

**INNNX. · Flutter 方块消除与战斗原型**

本仓库展示当前本地项目，源码保持私有。

## 当前实现

- 方块拖放、棋盘与消行逻辑。
- 史莱姆生命值与消行伤害计算。
- 按放置次数触发的敌方回合逻辑及攻击反馈组件。
- 本地音频、主题与持久化相关组件。

这些内容来自现有实现的静态检查；本次上传未重新运行游戏或验证发布构建，不代表完整成品。

## 技术栈

Flutter、Dart、Provider、SharedPreferences、flutter_animate、audioplayers；工程还包含截图和分享依赖。

## 现有截图

以下是本地保存的早期方块玩法截图，不展示后续史莱姆战斗界面：

<img src="screenshots/game.png" width="300" alt="早期方块玩法截图" />

## 项目来源与命名

本地原 README 标注了 Md Rounaq Ali 的 `block-crush-game` 项目；应用内部仍保留 Block Crush / block_blast 命名。本展示不将原项目内容全部归为 INNNX. 原创。上游来源与具体改动范围仍需进一步核实，因此不发布源码，不沿用原 README 的商店发布、性能或许可证声明。

## 公开范围

仅作品介绍和现有截图。应用源码、构建产物、开发环境配置与签名材料不公开。

当前战斗界面截图和实机演示尚待补充；分发前还需核实上游许可与素材使用范围。

---

## English

**INNNX. · A Flutter block-clearing and combat prototype**

This repository showcases the existing project. Application source code remains private.

### Current implementation
- Drag-and-drop blocks, board logic and line clearing.
- Slime health and damage calculations from cleared lines.
- Enemy turns triggered by placement counts, with attack feedback components.
- Local audio, themes and persistence components.

These descriptions come from the static inspection recorded in the existing README. The game and release builds have not been revalidated for this documentation update; this is not a claim of a finished product.

### Technology
Flutter, Dart, Provider, SharedPreferences, flutter_animate and audioplayers. The project also contains screenshot and sharing dependencies.

### Preview
The screenshot above shows an early block-game interface, not the later slime-combat interface. A current combat screenshot and gameplay recording have not yet been added.

### Origin and naming
The original local README credited Md Rounaq Ali's `block-crush-game` project. Internal names still include Block Crush / block_blast. This showcase does not attribute all upstream work to INNNX. The exact upstream source, modification scope and redistribution permissions still need verification. Source code is not published, and the original README's store-release, performance and license claims are not adopted here.

### Public scope and playable builds
Documentation and the existing screenshot only. Source code, build artifacts, development configuration and signing materials are excluded. No playable build is currently published here.

---

## Español

**INNNX. · Prototipo de eliminación de bloques y combate creado con Flutter**

Este repositorio presenta el proyecto existente. El código fuente de la aplicación permanece privado.

### Implementación actual
- Arrastrar y colocar bloques, lógica del tablero y eliminación de líneas.
- Vida del slime y cálculo del daño causado al eliminar líneas.
- Turnos del enemigo activados según el número de colocaciones y componentes de respuesta visual a los ataques.
- Componentes de audio local, temas y persistencia.

Estas descripciones proceden de la revisión estática indicada en el README existente. En esta actualización documental no se han vuelto a validar el juego ni las compilaciones de distribución; no se presenta como un producto terminado.

### Tecnología
Flutter, Dart, Provider, SharedPreferences, flutter_animate y audioplayers. El proyecto también incluye dependencias de captura de pantalla y de uso compartido.

### Vista previa
La captura superior muestra una interfaz temprana del juego de bloques, sin la interfaz posterior de combate contra slimes. Todavía no se han añadido una captura del combate actual ni una grabación de una partida.

### Origen y nombres
El README local original atribuía el proyecto `block-crush-game` a Md Rounaq Ali. La aplicación conserva nombres internos como Block Crush / block_blast. Esta presentación no atribuye todo el trabajo original a INNNX. Quedan por verificar el origen exacto, el alcance de las modificaciones y los permisos de redistribución. No se publica el código fuente ni se adoptan las afirmaciones del README original sobre tiendas, rendimiento o licencias.

### Alcance público y versiones jugables
Solo documentación y la captura existente. Se excluyen el código fuente, los archivos compilados, la configuración de desarrollo y los materiales de firma. Actualmente no se publica aquí una versión jugable.

---

[试玩发布说明 / Playable release guide / Guía de publicación](docs/PLAYABLE-RELEASE.md)
