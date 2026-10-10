# 试玩发布说明 / Playable release guide / Guía de publicación

## 中文

目前没有公开试玩包。本文件是后续发布准备说明，不是已发布或已验证的公告。

公开展示仓库可以发布经过验证的试玩包，同时保持开发仓库私有。GitHub 自动生成的 Source code ZIP/TAR 只是此展示仓库的文档与图片，不能当作游戏安装包。

### 发布前
1. 确认目标平台、版本、最低系统要求与安装方式，不因存在 Flutter 工程就宣称支持 Windows 或 iOS。
2. 用拟上传的同一文件在目标设备上验证安装、启动、核心玩法、退出与重新打开。记录设备、系统、测试日期和结果。
3. 核查包内没有密钥、签名私钥、本机路径、开发日志或其他私密材料；确认依赖、素材及上游项目允许该形式的分发。
4. 记录文件名、大小和 SHA-256，并列出已知问题、界面语言及网络需求。存在调试 APK 不等于已有可发布版本。
5. 包验证完成后，先准备 Release 草稿和测试记录，经用户确认再上传并公开。未验证的 APK/EXE 不上传。

### 发布说明填写模板
- 版本、发布日期、试玩范围。
- 平台、最低系统要求、安装与卸载方法。
- 界面语言、联网需求、广告或内购在此试玩中的实际行为。
- 已验证项目：测试设备、系统、日期、结果。
- 已知问题和未验证平台。
- 资产：文件名、大小、SHA-256。
- 反馈：通过本展示仓库的 Issues 提交设备信息、复现步骤和必要截图，请勿附个人资料。
- 源码保持私有；发行包的使用条款与适用第三方声明另行确认。

### 截图和演示计划
保留现有真实截图及版本说明。补充实际运行得到的首页、核心玩法、结果或失败状态；仅在真实验证后添加英语和西语界面截图。录制约 20–40 秒连续操作演示，标明版本和平台，避免个人信息、调试覆盖层和开发路径。没有实机素材时不制作冒充游戏画面的图片。

## English

No playable package is currently public. This document prepares a future release; it is not a release announcement or evidence of build validation.

A public showcase can host a verified playable package while the development repository stays private. GitHub's automatically generated Source code ZIP/TAR contains this showcase's documentation and images, not a game installer.

### Before publication
1. Confirm the platform, version, minimum system requirements and installation steps. A Flutter project alone does not establish Windows or iOS support.
2. Test the exact upload candidate on the target device: install, launch, core gameplay, exit and reopen. Record device, OS, test date and results.
3. Check for secrets, signing private keys, local paths, development logs and other private material. Verify redistribution permissions for dependencies, assets and upstream work.
4. Record filename, size and SHA-256, known issues, interface languages and network requirements. A debug APK is not automatically a publishable build.
5. Once verified, prepare a Release draft and test record; obtain the user's confirmation before uploading and publishing. Do not upload unverified APK/EXE files.

### Release-note fields
Version and date; demo scope; platform and minimum requirements; installation and removal; interface languages; network needs; actual ad/purchase behavior; tested devices, OS, dates and results; known issues and untested platforms; asset filename, size and SHA-256; feedback through this repository's Issues without personal information; private-source status and confirmed distribution terms/third-party notices.

### Screenshot and demo plan
Keep the existing authentic screenshot and version context. Add real captures of the home screen, core gameplay and results or failure states. Add English/Spanish interface captures only after checking those screens. Record roughly 20–40 seconds of continuous interaction with version/platform context, without personal information, debug overlays or development paths. Do not fabricate gameplay imagery.

## Español

Actualmente no hay un paquete jugable público. Este documento prepara una futura publicación; no anuncia una versión publicada ni acredita su validación.

Un repositorio público de presentación puede alojar un paquete jugable verificado mientras el repositorio de desarrollo sigue privado. Los archivos Source code ZIP/TAR generados automáticamente por GitHub contienen la documentación y las imágenes de esta presentación, no un instalador del juego.

### Antes de publicar
1. Confirmar plataforma, versión, requisitos mínimos e instalación. Un proyecto de Flutter no demuestra por sí solo compatibilidad con Windows o iOS.
2. Probar el mismo archivo que se pretende subir: instalación, inicio, mecánica principal, salida y reapertura. Registrar dispositivo, sistema, fecha y resultados.
3. Revisar que no incluya secretos, claves privadas de firma, rutas locales, registros de desarrollo ni otros datos privados. Verificar los permisos de redistribución de dependencias, recursos y proyecto original.
4. Registrar nombre, tamaño y SHA-256, problemas conocidos, idiomas de interfaz y requisitos de conexión. Un APK de depuración no equivale a una versión lista para publicar.
5. Tras verificar el paquete, preparar un borrador de Release y el registro de pruebas; obtener la confirmación del usuario antes de subirlo y publicarlo. No subir APK/EXE sin verificar.

### Campos de las notas de versión
Versión y fecha; alcance de la demo; plataforma y requisitos mínimos; instalación y desinstalación; idiomas; conexión; comportamiento real de anuncios/compras; dispositivos, sistemas, fechas y resultados de pruebas; problemas conocidos y plataformas no verificadas; nombre, tamaño y SHA-256 del archivo; comentarios mediante Issues sin datos personales; código privado y condiciones de distribución/avisos de terceros confirmados.

### Plan de capturas y demostración
Conservar la captura auténtica y su contexto de versión. Añadir capturas reales del inicio, la mecánica principal y los resultados o estados de derrota. Añadir pantallas en inglés/español solo después de verificarlas. Grabar unos 20–40 segundos de interacción continua indicando versión/plataforma, sin datos personales, superposiciones de depuración ni rutas de desarrollo. No fabricar imágenes de partidas.

## BlockSlayer

发布门槛：先核实 Md Rounaq Ali / `block-crush-game` 的具体上游来源、许可及素材分发权限。 / Release prerequisite: verify the exact upstream source, license and asset redistribution permissions. / Requisito previo: verificar el origen exacto, la licencia y los permisos de redistribución de los recursos.
