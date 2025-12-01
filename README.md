
<p align="left"><img src="icon.jpg"></p>

# <b>Linkalho</b>

Linkalho 是一款自制软件，可以离线关联 NNID 账号。它可以关联（或取消关联）<b>现有</b>账号，因此您不会丢失存档。

此应用不会创建新账号。如果您创建了新账号并想要关联，只需重新运行此应用即可。

<br>

## <b>我为什么需要这个应用？</b>

如果您从未遇到过游戏/应用在关联 Switch 用户账号前无法启动的问题，也从未遇到过某些游戏卡在“正在更新游戏数据”界面，或者某些官方模拟器只显示黑屏而不显示游戏选择界面的问题，那么您无需使用此自制软件。

<br>

你喜欢这个应用吗？觉得它实用吗？你可以点击下面的链接请我喝杯咖啡。谢谢！(该打赏链接为原作者链接，非本译者链接)<br>
<a href="https://paypal.me/rdmrocha"><img src="raw/buy-me-a-coffee.png" width="150px" /></a>

<br>

## <b>常见问题解答</b>：

- 为什么我无法通过触摸屏或拇指勾选来操作应用？

- 这是一个非常简单易用的应用，大多数用户只会使用一两次。除非 Borealis 的开发者原生支持此功能，否则我没有计划扩展其功能集。

- 我可以使用虚假/生成的关联账户上网吗？

- 不行！您的 Switch 已被破解。上网始终存在风险。

- 这个应用可以“在此处提问”吗？

- 您可以先阅读[上一节](https://github.com/rdmrocha/linkalho#why-do-i-need-this-app)。此应用允许您在无需网络连接的情况下将虚假/生成的 NNID 关联/取消关联到您的用户账户，仅此而已。如果您仍然不理解这是什么以及它的用途，那么您很可能根本不需要此应用。别担心：如果你需要它，你自然会知道。

<br>

## <b>安装</b>：

- 将 .nro 文件放入 SD 卡的 `/switch/linkalho` 文件夹中。

- 打开 Homebrew 应用并运行 Linkalho。

<br>

### <u>重启到有效载荷</u>

完成所选操作后，如果满足以下条件，Linkalho 将重启到现有有效载荷：

- 主机硬件为 Erista，且用户将有效载荷文件放置在应用程序根目录（`/switch/linkalho/reboot.bin`）。

Mariko 硬件不支持重启到有效载荷！
<br>

## <b>用法</b>:

### <u>关联选定账户</u>

- 将关联控制台上所有选定的账户。如果任何现有账户已关联，则会重新关联（无论 NNID 是否已正式关联）。

此操作会在 `/switch/linkalho/backups` 目录下创建备份。

### <u>取消关联选定账户</u>

- 将从控制台上任何选定的账户中移除 NNID 关联，无论 NNID 是否已正式关联。

此操作会在 `/switch/linkalho/backups` 目录下创建备份。

### <u>恢复备份</u>

- 从备份文件恢复任何先前的状态。该文件必须位于 `/switch/linkalho/restore/restore.zip` 目录下。如果该文件不存在，用户界面将通知用户。

此操作会在 `/switch/linkalho/backups` 目录下创建备份。

### <u>创建手动备份</u>

- 将在 `/switch/linkalho/backups` 目录下创建备份。

所有链接和取消链接操作都会在进行更改之前自动生成备份。

<b>仅当您想手动创建备份时才应使用此选项！</b>

### <u>选择链接帐户的国家/地区</u>

- 允许用户自定义要添加到链接帐户的国家/地区。这会影响某些软件，例如显示相应的标志（例如在 mk8 中）。

### <u>选择要链接/取消链接的帐户</u>

- 允许用户选择要链接/取消链接的帐户。默认值为**_all__**。如果未选择任何帐户，并且用户尝试执行链接或取消链接操作，应用程序将显示错误。

<br>

## <b>Screenshots</b>
<p align="center"><img src="raw/screenshot1.jpg"></p>
<p align="center"><img src="raw/screenshot2.jpg"></p>
<p align="center"><img src="raw/screenshot3.jpg"></p>
<p align="center"><img src="raw/screenshot4.jpg"></p>
<p align="center"><img src="raw/screenshot5.jpg"></p>
<p align="center"><img src="raw/screenshot6.jpg"></p>
<p align="center"><img src="raw/screenshot7.jpg"></p>
<p align="center"><img src="raw/screenshot8.jpg"></p>
<p align="center"><img src="raw/screenshot9.jpg"></p>
<p align="center"><img src="raw/screenshot10.jpg"></p>
<p align="center"><img src="raw/screenshot11.jpg"></p>

<br>

## <b>Credits</b>
  - [devkitPro](https://devkitpro.org) for the toolchain!
  - [natinusala (lib borealis)](https://github.com/natinusala/borealis) for the amazing library that mimicks the Switch's original UI and UX
  - [sebastiandev (zipper wrapper for minizip)](https://github.com/sebastiandev/zipper/) for their nice wrapper to the minizip
  - [Kronos2308](https://github.com/Kronos2308) for the help in the initial phases of research.
  - [SciresM](https://github.com/SciresM) for his "reboot to payload" code and [HamletDuFromage](https://github.com/HamletDuFromage) for the code contributions
  - **target** for the icon, the beta testing and for supplying crucial files that helped in the creation of the generators.
  - **boredomisacrime** for the beta testing.
