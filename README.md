# <img align="center" height="70" src="./Docs/Images/AppIcon.png"/> GitHub Copilot for Xcode

[GitHub Copilot](https://github.com/features/copilot) for Xcode is the leading AI coding assistant for Swift, Objective-C and iOS/macOS development. It delivers intelligent Completions, Chat, and Code Review—plus advanced features like Agent Mode, Next Edit Suggestions, MCP Registry, and Copilot Vision to make Xcode development faster and smarter.

> [!IMPORTANT]  
> Starting from version v0.50.0, we have added internal support for the upcoming usage-based billing experience, including experience updates to the usage panel, usage notifications, and model picker. These changes will become visible once usage-based billing is rolled out. 
> 
> To ensure compatibility with the new billing experience, we strongly recommend upgrading to the latest plugin version as soon as possible: 
> 
> * **GitHub Copilot for Xcode: v0.50.0 or later**
> 
> Clients using older plugin versions will continue to function. However, the billing and usage experience may not be optimal and may not accurately reflect the latest usage-based billing experience. 

## Chat

GitHub Copilot Chat provides suggestions to your specific coding tasks via chat.
<img alt="Chat of GitHub Copilot for Xcode" src="./Docs/Images/chat_agent.gif" width="800" />

## Agent Mode

GitHub Copilot Agent Mode provides AI-powered assistance that can understand and modify your codebase directly. With Agent Mode, you can:
- Get intelligent code edits applied directly to your files
- Run terminal commands and view their output without leaving the interface
- Search through your codebase to find relevant files and code snippets
- Create new files and directories as needed for your project
- Get assistance with enhanced context awareness across multiple files and folders
- Run Model Context Protocol (MCP) tools you configured to extend the capabilities

Agent Mode integrates with Xcode's environment, creating a seamless development experience where Copilot can help implement features, fix bugs, and refactor code with comprehensive understanding of your project.

## Code Completion

You can receive auto-complete type suggestions from GitHub Copilot either by starting to write the code you want to use, or by writing a natural language comment describing what you want the code to do.
<img alt="Code Completion of GitHub Copilot for Xcode" src="./Docs/Images/demo.gif" width="800" />

## Requirements

- macOS 13+
- Xcode 14+
- A GitHub account

## Getting Started

1. Install via [Homebrew](https://brew.sh/):

   ```sh
   brew install --cask github-copilot-for-xcode
   ```

   Or download the `dmg` from
   [the latest release](https://github.com/github/CopilotForXcode/releases/latest/download/GitHubCopilotForXcode.dmg).
   Drag `GitHub Copilot for Xcode` into the `Applications` folder:

   <p align="center">
     <img alt="Screenshot of opened dmg" src="./Docs/Images/dmg-open.png" width="512" />
   </p>

   Updates can be downloaded and installed by the app.

1. Open the `GitHub Copilot for Xcode` application (from the `Applications` folder). Accept the security warning.
   <p align="center">
     <img alt="Screenshot of MacOS download permission request" src="./Docs/Images/macos-download-open-confirm.png" width="350" />
   </p>


1. A background item will be added to enable the GitHub Copilot for Xcode extension app to connect to the host app. This permission is usually automatically added when first launching the app.
   <p align="center">
     <img alt="Screenshot of background item" src="./Docs/Images/background-item.png" width="370" />
   </p>

1. Three permissions are required for GitHub Copilot for Xcode to function properly: `Background`, `Accessibility`, and `Xcode Source Editor Extension`. For more details on why these permissions are required see [TROUBLESHOOTING.md](./TROUBLESHOOTING.md).

   The first time the application is run the `Accessibility` permission should be requested:

   <p align="center">
     <img alt="Screenshot of accessibility permission request" src="./Docs/Images/accessibility-permission-request.png" width="529" />
   </p>

   The `Xcode Source Editor Extension` permission needs to be enabled manually. Click
   `Extension Permission` from the `GitHub Copilot for Xcode` application settings to open the
   System Preferences to the `Extensions` panel. Select `Xcode Source Editor`
   and enable `GitHub Copilot`:

   <p align="center">
     <img alt="Screenshot of extension permission" src="./Docs/Images/extension-permission.png" width="582" />
   </p>

1. After granting the extension permission, open Xcode. Verify that the
   `Github Copilot` menu is available and enabled under the Xcode `Editor`
   menu.
    <br>
    <p align="center">
      <img alt="Screenshot of Xcode Editor GitHub Copilot menu item" src="./Docs/Images/xcode-menu.png" width="648" />
    </p>

    Keyboard shortcuts can be set for all menu items in the `Key Bindings`
    section of Xcode preferences.

1. To sign into GitHub Copilot, click the `Sign in` button in the settings application. This will open a browser window and copy a code to the clipboard. Paste the code into the GitHub login page and authorize the application.
    <p align="center">
      <img alt="Screenshot of sign-in popup" src="./Docs/Images/device-code.png" width="372" />
    </p>

1. To install updates, click `Check for Updates` from the menu item or in the
   settings application.

   After installing a new version, Xcode must be restarted to use the new
   version correctly.

   New versions can also be installed from `dmg` files downloaded from the
   releases page. When installing a new version via `dmg`, the application must
   be run manually the first time to accept the downloaded from the internet
   warning.

1. To avoid confusion, we recommend disabling `Predictive code completion` under
   `Xcode` > `Preferences` > `Text Editing` > `Editing`.

1. Press `tab` to accept the first line of a suggestion, hold `option` to view
   the full suggestion, and press `option` + `tab` to accept the full suggestion.

## How to use Chat

   Open Copilot Chat in GitHub Copilot.
  - Open via the Xcode menu `Xcode -> Editor -> GitHub Copilot -> Open Chat`.
  <p align="center">
    <img alt="Screenshot of Xcode Editor GitHub Copilot menu item" src="./Docs/Images/xcode-menu_dark.png" width="648" />
  </p>

  - Open via GitHub Copilot app menu `Open Chat`.

  <p align="center">
    <img alt="Screenshot of GitHub Copilot menu item" src="./Docs/Images/copilot-menu_dark.png" width="244" />
  </p>

## How to use Code Completion

   Press `tab` to accept the first line of a suggestion, hold `option` to view
   the full suggestion, and press `option` + `tab` to accept the full suggestion.

## License

This project is licensed under the terms of the MIT open source license. Please
refer to [LICENSE.txt](./LICENSE.txt) for the full terms.

## Privacy

We follow responsible practices in accordance with our
[Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-privacy-statement).

To get the latest security fixes, please use the latest version of the GitHub
Copilot for Xcode.

## Support

We’d love to get your help in making GitHub Copilot better!  If you have
feedback or encounter any problems, please reach out on our [Feedback
forum](https://github.com/github/CopilotForXcode/discussions).

## Acknowledgements

Thank you to @intitni for creating the original project that this is based on.

Attributions can be found under About when running the app or in
[Credits.rtf](./Copilot%20for%20Xcode/Credits.rtf).

func calculateDaysBetweenDates(
# IDE 中GitHub Copilot 的键盘快捷方式

查找在支持的 IDE 中 GitHub Copilot 的键盘快捷方式列表。

<div class="ghd-tool jetbrains">

使用 GitHub Copilot 时，可以在 JetBrains IDE 中使用默认键盘快捷方式获取内联建议。

## macOS 键盘快捷方式

| 动作 | 快捷键 |
|:---|:---|
|接受内联建议|
<kbd>选项卡</kbd>|
|忽略内联建议|
<kbd>Esc</kbd>|
|显示下一个内联建议|
<kbd>Option (⌥) 或 Alt</kbd>+<kbd>]</kbd>|
|显示上一个内联建议|
<kbd>Option (⌥) 或 Alt</kbd>+<kbd>[</kbd>|
|触发内联建议|
<kbd>选项 (⌥)</kbd>+<kbd>\\</kbd>|
|打开 GitHub Copilot（在单独的面板中查看其他建议）|
<kbd>Option (⌥) 或 Alt</kbd>+<kbd>返回</kbd> |

## Windows 键盘快捷方式

| 动作 | 快捷键 |
|:---|:---|
|接受内联建议|
<kbd>选项卡</kbd>|
|忽略内联建议|
<kbd>Esc</kbd>|
|显示下一个内联建议|
<kbd>Alt</kbd>+<kbd>]</kbd>|
|显示上一个内联建议|
<kbd>Alt</kbd>+<kbd>[</kbd>|
|触发内联建议|
<kbd>Alt</kbd>+<kbd>\\</kbd>|
|打开 GitHub Copilot（在单独的面板中查看其他建议）|
<kbd>Alt</kbd>+<kbd>进入</kbd> |

## Linux 键盘快捷方式

| 动作 | 快捷键 |
|:---|:---|
|接受内联建议|
<kbd>选项卡</kbd>|
|忽略内联建议|
<kbd>Esc</kbd>|
|显示下一个内联建议|
<kbd>Alt</kbd>+<kbd>]</kbd>|
|显示上一个内联建议|
<kbd>Alt</kbd>+<kbd>[</kbd>|
|触发内联建议|
<kbd>Alt</kbd>+<kbd>\\</kbd>|
|打开 GitHub Copilot（在单独的面板中查看其他建议）|
<kbd>Alt</kbd>+<kbd>进入</kbd> |

</div>

<div class="ghd-tool visualstudio">

使用 Visual Studio 时，可使用 GitHub Copilot 中的内联建议的默认键盘快捷方式。 可以在键盘快捷方式编辑器中按命令名称搜索每个键盘快捷方式。

| 动作 | 快捷键 | 命令名称 |
|:---|:---|:---|
|显示下一个内联建议|
<kbd>Alt</kbd>+<kbd>。</kbd>|编辑.下一个建议|
|显示上一个内联建议|
<kbd>Alt</kbd>+<kbd>、</kbd>|Edit.PreviousSuggestion|

</div>

<div class="ghd-tool vscode">

您可以在 GitHub Copilot 中使用 Visual Studio Code 的默认键盘快捷方式。 在键盘快捷方式编辑器中，按命令名称搜索键盘快捷方式。

## macOS 键盘快捷方式

| 动作 | 快捷键 | 命令名称 |
|:---|:---|:---|
|接受内联建议|
<kbd>选项卡</kbd>|editor.action.inlineSuggest.commit|
|忽略内联建议|
<kbd>Esc</kbd>|editor.action.inlineSuggest.hide|
|显示下一个内联建议| 
<kbd>选项 （⌥）</kbd>+<kbd>]</kbd><br> |editor.action.inlineSuggest.showNext|
|显示上一个内联建议| 
<kbd>选项 （⌥）</kbd>+<kbd>[</kbd><br> |editor.action.inlineSuggest.showPrevious|
|触发内联建议| 
<kbd>选项 (⌥)</kbd>+<kbd>\\</kbd><br> |editor.action.inlineSuggest.trigger|
|打开 GitHub Copilot（在单独的面板中查看其他建议）|
<kbd>Ctrl</kbd>+<kbd>返回</kbd>|github.copilot.generate|
|开启/关闭 GitHub Copilot|没有默认快捷方式|github.copilot.toggleCopilot|

## Windows 键盘快捷方式

| 动作 | 快捷键 | 命令名称 |
|:---|:---|:---|
|接受内联建议|
<kbd>选项卡</kbd>|editor.action.inlineSuggest.commit|
|忽略内联建议|
<kbd>Esc</kbd>|editor.action.inlineSuggest.hide|
|显示下一个内联建议|
<kbd>Alt</kbd>+<kbd>]</kbd> |editor.action.inlineSuggest.showNext|
|显示上一个内联建议|
<kbd>Alt</kbd>+<kbd>[</kbd>|editor.action.inlineSuggest.showPrevious|
|触发内联建议|
<kbd>Alt</kbd>+<kbd>\\</kbd>|editor.action.inlineSuggest.trigger|
|打开 GitHub Copilot（在单独的面板中查看其他建议）|
<kbd>Ctrl</kbd>+<kbd>进入</kbd>|github.copilot.generate|
|开启/关闭 GitHub Copilot|没有默认快捷方式|github.copilot.toggleCopilot|

## Linux 键盘快捷方式

| 动作 | 快捷键 | 命令名称 |
|:---|:---|:---|
|接受内联建议|
<kbd>选项卡</kbd>|editor.action.inlineSuggest.commit|
|忽略内联建议|
<kbd>Esc</kbd>|editor.action.inlineSuggest.hide|
|显示下一个内联建议|
<kbd>Alt</kbd>+<kbd>]</kbd> |editor.action.inlineSuggest.showNext|
|显示上一个内联建议|
<kbd>Alt</kbd>+<kbd>[</kbd>|editor.action.inlineSuggest.showPrevious|
|触发内联建议|
<kbd>Alt</kbd>+<kbd>\\</kbd>|editor.action.inlineSuggest.trigger|
|打开 GitHub Copilot（在单独的面板中查看其他建议）|
<kbd>Ctrl</kbd>+<kbd>进入</kbd>|github.copilot.generate|
|开启/关闭 GitHub Copilot|没有默认快捷方式|github.copilot.toggleCopilot|

</div>

<div class="ghd-tool xcode">

使用 GitHub Copilot 时，可以在 Xcode 中使用默认键盘快捷方式获取内联建议。 或者，可以将快捷方式重新绑定到每个特定命令的首选键盘快捷方式。

| 动作 | 快捷键 |
|:---|:---|
|接受建议的第一行|
<kbd>选项卡</kbd>|
|查看完整建议|按住 <kbd>Option</kbd>|
|接受完整建议|
<kbd>选项</kbd>+<kbd>选项卡</kbd>|

</div>

<div class="ghd-tool eclipse">

使用 GitHub Copilot 时，可以在 Eclipse 中使用默认键盘快捷方式获取内联建议。

| 动作 | 快捷键 |
|:---|:---|
|接受内联建议|
<kbd>选项卡</kbd>|
|接受内联建议的下一个词|
<kbd>Command</kbd>+<kbd>&rarr;</kbd> (Mac) 或 <kbd>Ctrl</kbd>+<kbd>&rarr;</kbd> (Windows)|
|忽略内联建议|
<kbd>Esc</kbd>|
|触发内联建议|
<kbd>Option (⌥)</kbd>+<kbd>Command</kbd>+<kbd>/</kbd> (Mac) 或 <kbd>Alt</kbd>+<kbd>Ctrl</kbd>+<kbd>/</kbd> (Windows)|

</div>

<div class="ghd-tool vimneovim">

使用 GitHub Copilot 为每个特定命令使用首选键盘快捷方式时，可以在 Vim/Neovim 中重新绑定键盘快捷方式。 有关详细信息，请参阅 Neovim 文档中的[映射](https://neovim.io/doc/user/map.html)一文。

</div>  - name: 'Upload Artifact'
    uses: actions/upload-artifact@v4
    with:
      name: my-artifact
      path: my_file.txt
      retention-days: 5
# GitHub CLI api
# https://cli.github.com/manual/gh_api

gh api \
  --method PUT \
  -H "Accept: application/vnd.github+json" \
  -H "X-GitHub-Api-Version: 2026-03-10" \
  /repos/OWNER/REPO/actions/permissions/workflow \
   -f 'default_workflow_permissions=read' -F "can_approve_pull_request_reviews=true"

  - name: Set up Go
    uses: actions/setup-go@4a3601121dd01d1626a1e23e37211e3254c1c06c # v6.4.0
    with:
      go-version: "stable"

  - name: Run govulncheck
    run: |
      make -C validator govulncheck

  # TODO: Publish releases
  - name: Build
    run: make validator

  - name: Test
    run: |
      cd validator
      go test .

  - name: Run ShellTests
    run: |
      make validator"指紋：5AA568620F4EC889AFF7A8A9826FADFF59548BFC
Uid: Alberto Bertogli <albertito@blitiri.com.ar>
允許：chasquid（43673975973406E650A64124CF0E265B7DFBB2F2），
 kxd (F8921D3A7404C86E11352215C7197699B29B232A)

指紋：487FCD050895105F43C206089B2E6B82752DB03B
Uid：Alberto Luaces Fernández <aluaces@udc.es>
允許：openscenegraph（2A8E80505C486298430DD0937F7606A445DCA80E），
 openscenegraph-3.4 (2A8E80505C486298430DD0937F7606A445DCA80E)

指紋：E2EA41DCE2F8A99AD17A1E463A67D5D966D15C5C
使用者 ID：Alec Leamas <leamas.alec@gmail.com>
允許：ddupdate (92978A6E195E4921825F7FF0F34F09744E9F5DD9)
 libcxx-serial（13C904F0CE085E7C36307985DECF849AA6357FB7），
 lirc（13C904F0CE085E7C36307985DECF849AA6357FB7），
 lirc-compat-remotes (13C904F0CE085E7C36307985DECF849AA6357FB7)
 opencpn (13C904F0CE085E7C36307985DECF849AA6357FB7),
 wxsvg (2861257317C7AEE4F880497EC3860AC59F574E3A)

指紋：2875F6B1C2D27A4F0C8AF60B2A714497E37363AE
Uid：Aleksey Kravchenko <rhash.admin@gmail.com>
允許：libpff（BFAE9E331A867A7C80D8EB78F4E4ACDBB8D08BE0），
 rhash (BFAE9E331A867A7C80D8EB78F4E4ACDBB8D08BE0)

指紋：4CF4B452C6F986EEBA0F17F5972AF09CFECEEACE
Uid：Alexandre Rossi <niol@zincube.net>
允許：davmail (8A7F208C6D9E73291657414D2135D123D8C19BEC)
 gnome-shell-extension-paperwm (4D0BE12F0E4776D8AACE9696E66C775AEBFE6C7D)
 石墨網（A0B1A9F3508956130E7A425CD416AD15AC6B43FE），
 懶惰加爾（63CB1DF1EF12CF2AC0EE5A329C27B31342B7511D），
 libhtmlcleaner-java (8A7F208C6D9E73291657414D2135D123D8C19BEC)

指紋：B738B2973EE4E0D47A4A3B185A7BAB1891FDFA61
Uid： Alexandre Viard <xela@viard.dev>
允許：81伏（796DB393DC3FF40222B6EA22D3EBB5966BB99196）

指紋：AA222B227899319ECA3C1A364AD58E3068E669E2
Uid：Alexis Bienvenüe <pado@passoire.fr>
允許：自動多選 (3340B364FF67153FB7CCAE851C2816907136AE39)

指紋：B7E60EBB92937B06BDBC2787E7BD1904F480937F
Uid：Alexis Murzeau <amubtdx@gmail.com>
允許：streamlink (D3F0E02EC45A938E1D67229EC43496655925B604)

指紋：54351AAF3F6C43D35C52CF6CA8696F011940D6C7
Uid：Alkis Georgopoulos <alkisg@gmail.com>
允許：epoptes (F0ADA5240891831165DF98EA7CFCD8CD257721E9)，
 ldm (F0ADA5240891831165DF98EA7CFCD8CD257721E9),
 ltsp（F0ADA5240891831165DF98EA7CFCD8CD257721E9），
 ltsp-docs（F0ADA5240891831165DF98EA7CFCD8CD257721E9），
 ltspfs (F0ADA5240891831165DF98EA7CFCD8CD257721E9)

指紋：F225BB6B5A9B18FF331DFAF6C32A4D0858F5A6EA
Uid：Alper Nebi Yasak <alpernebiyasak@gmail.com>
允許：深水炸彈工具（03C4E7ABB880F524306E48156611C05EDD39F374），
 depthcharge-tools-installer (B60EBF2984453C70D74CF478FF914AF0C2B35520)
 partman-cros (B60EBF2984453C70D74CF478FF914AF0C2B35520)

指紋：6EED8674F8A1557A057382AAD74D4EE0580CA4FC
使用者 ID：Andreas Dolp <mail@andreas-dolp.de>
允許：libhtp（0EED77DC41D760FDE44035FF5556A34E04A3610B），
 suricata (0EED77DC41D760FDE44035FF5556A34E04A3610B),
 suricata-update (0EED77DC41D760FDE44035FF5556A34E04A3610B)

指紋：74CDD9FE5BCBFE0D13EE8EEA61F3442674DE6624
使用者 ID：Andreas Moog <andreas.moog@warperbbs.de>
允許：elycharts.js (F78CBA07817BB149A11D339069F2FC516EA71993)
 libpar2 (F78CBA07817BB149A11D339069F2FC516EA71993),
 nzbget (F78CBA07817BB149A11D339069F2FC516EA71993),
 pdfcube (F78CBA07817BB149A11D339069F2FC516EA71993)

指紋：1662F3FE0EF53DE5E6CE0031B446EEA8329A945A
使用者 ID：Andreas Noteng <andreas@noteng.no>
允許：檢查安裝（218EE0362033C87B6C135FA4A3BABAE2408DD6CF），
 pype (08E2400FF7FE8FEDE3ACB52818147B073BAD2B07)
 pyspread（D53A815A3CB7659AF882E3958EEDCC1BAA1F32FF），
 python-easygui (8F6DE104377F3B11E741748731F3144544A1741A)
 transgui (374FF2AD0A12935FD0B0C84F1B132E01CEC6AD46)

指紋：06AB786E936C6C73F6D8130C4510339430FC9F34
使用者 ID：Andrew Bower <andrew@bower.org.uk>
允許:getdns(4A5FD1CD115087CC03DC35C1D597897206C5F07F),
 mcds（14593BFF4A5EBF6FE0E9716EECBEDBB607B9B2BE），
 金屬（B8FAC2E250475B8CE940A91957930DAB0B86B067），
 popa3d（F1F007320A035541F0A663CA578A0494D1C646D1），
 shellinabox（F1F007320A035541F0A663CA578A0494D1C646D1），
 sysv-rc-conf (14593BFF4A5EBF6FE0E9716EECBEDBB607B9B2BE)
 wtmpdb (7D1ACFFAD9E0806C9C4CD3925C13D6DB93052E03),
 xchpst (14593BFF4A5EBF6FE0E9716EECBEDBB607B9B2BE)

指紋：76C282AB9B59447C39B7CEEA0576302FE189D4D2
Uid：Andriy Grytsenko <andrej@rep.kiev.ua>
允許：foxeye (BBBD45EA818AB86FF67E7285D3E17383CFA7FF06)
 gnome-system-tools (BBBD45EA818AB86FF67E7285D3E17383CFA7FF06)
 libfm（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 liboob（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lx外觀（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lxappearance-obconf（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lxde-common（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lxde-icon-theme（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lxde-metapackages（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lxdm（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lxhotkey（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lx輸入（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lx啟動器（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lxmenu-data（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lx音樂（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lx面板（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lxrandr（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lx會話（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lxtask（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 lxterminal（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 選單快取（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 pcmanfm（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 系統工具後端 (BBBD45EA818AB86FF67E7285D3E17383CFA7FF06)

指紋：2A341FB6601406C144ADEEE4C4C3F43EC6F0514F
Uid：Aniol Martí <aniol@aniolmarti.cat>
允許：aegisub (6940702AC6DEB565B648A4EDE3AE978E834E5E7E),
 電路宏（6940702AC6DEB565B648A4EDE3AE978E834E5E7E），
 dpic（6940702AC6DEB565B648A4EDE3AE978E834E5E7E），
 openvpn-auth-ldap (6940702AC6DEB565B648A4EDE3AE978E834E5E7E),
 pycirkuit (6940702AC6DEB565B648A4EDE3AE978E834E5E7E)

指紋：254571A4BCA37CC36B9BB498922C1B66A3D3D022
使用者 ID：Antonin Delpeuch <antonin@delpeuch.eu>
允許: rust-ambient-id (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 rust-astral-async-http-range-reader（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8）
 rust-astral-pubgrub（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-astral-reqwest-retry (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 rust-astral-version-ranges (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 rust-async-http-range-reader（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8）
 rust-citationberg（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-cyclonedx-bom（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 銹-diffy-imara (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 rust-ecow（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-git-conventional（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-integer-sqrt (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 rust-libxml（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-lipsum（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-markdown（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-nanoid（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-next-version (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 rust-nonempty-collections（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 銹一次性（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-pathfinding（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-priority-queue（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-qcms（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-reqsign-core（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-reqsign-file-read-tokio (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 rust-reqsign-http-send-reqwest (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8)
 rust-retry-policies（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-rmpv（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-spdx（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-streaming-iterator（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 rust-tree-edit-distance (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 tree-sitter-bash (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 tree-sitter-go (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 樹保姆-ini (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 tree-sitter-json（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 tree-sitter-php（9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8），
 tree-sitter-powershell (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8)
 tree-sitter-ruby (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 tree-sitter-rust-orchard (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 tree-sitter-yaml (9284B15F1D56DD78BC1B62B157D77C19CCFD1EF8),
 uv (772292F6F7AC85FAE041D41EE5F43F9C2734F287)

指紋：3B70F209A5FFD68903C472C5EBF48AB2578F9812
Uid：安東尼奧·瓦倫蒂諾 <antonio.valentino@tiscali.it>
允許：aggdraw（8182DE417056408D614650D16750F10AE88D4AF1），
 反甲硝唑（8182DE417056408D614650D16750F10AE88D4AF1），
 asciitree（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 asf-search (8182DE417056408D614650D16750F10AE88D4AF1),
 asfsmd（8182DE417056408D614650D16750F10AE88D4AF1），
 bpack（8182DE417056408D614650D16750F10AE88D4AF1），
 c-blosc2 (E92E7E6E9E9DA6B1AA3139DC5632906F4696E015),
 cdsetool（8182DE417056408D614650D16750F10AE88D4AF1），
 編譯（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 cyarray（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 dask-影像（8182DE417056408D614650D16750F10AE88D4AF1），
 donfig（8182DE417056408D614650D16750F10AE88D4AF1），
 doris（8182DE417056408D614650D16750F10AE88D4AF1），
 ecmwf-api-client（8182DE417056408D614650D16750F10AE88D4AF1），
 eodag (8182DE417056408D614650D16750F10AE88D4AF1),
 epr-api（8182DE417056408D614650D16750F10AE88D4AF1），
 fiona (8182DE417056408D614650D16750F10AE88D4AF1),
 flexcache（A0B1A9F3508956130E7A425CD416AD15AC6B43FE），
 flexparser（A0B1A9F3508956130E7A425CD416AD15AC6B43FE），
 flox（8182DE417056408D614650D16750F10AE88D4AF1），
 甘油 (8182DE417056408D614650D16750F10AE88D4AF1),
 gmtsar（8182DE417056408D614650D16750F10AE88D4AF1），
 jplephem (3E99A526F5DCC0CBBF1CEEA600BAE74B343369F1),
 jsonpath-ng (8182DE417056408D614650D16750F10AE88D4AF1),
 kerchunk (8182DE417056408D614650D16750F10AE88D4AF1),
 lerc (8182DE417056408D614650D16750F10AE88D4AF1),
 mapraster（8182DE417056408D614650D16750F10AE88D4AF1），
 metpy（8182DE417056408D614650D16750F10AE88D4AF1），
 mintpy（8182DE417056408D614650D16750F10AE88D4AF1），
 morecantile (8182DE417056408D614650D16750F10AE88D4AF1),
 numcodecs（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 numexpr (BBBD45EA818AB86FF67E7285D3E17383CFA7FF06),
 pathlib-abc (8182DE417056408D614650D16750F10AE88D4AF1),
 pims（8182DE417056408D614650D16750F10AE88D4AF1），
 pint-xarray（8182DE417056408D614650D16750F10AE88D4AF1），
 小狗（8182DE417056408D614650D16750F10AE88D4AF1），
 pyaps3 (8182DE417056408D614650D16750F10AE88D4AF1),
 pycoast（8182DE417056408D614650D16750F10AE88D4AF1），
 pydecorate（8182DE417056408D614650D16750F10AE88D4AF1），
 pyepr（8182DE417056408D614650D16750F10AE88D4AF1），
 pyerfa (BAFC6C85F7CB143FEEB6FB157115AFD07710DCF7)
 pygac（8182DE417056408D614650D16750F10AE88D4AF1），
 pygeofilter（8182DE417056408D614650D16750F10AE88D4AF1），
 pykdtree（8182DE417056408D614650D16750F10AE88D4AF1），
 pykml（8182DE417056408D614650D16750F10AE88D4AF1），
 pylibtiff (8182DE417056408D614650D16750F10AE88D4AF1),
 pymap3d（8182DE417056408D614650D16750F10AE88D4AF1），
 pyninjotiff (8182DE417056408D614650D16750F10AE88D4AF1),
 pyogrio (8182DE417056408D614650D16750F10AE88D4AF1),
 pyorbital（8182DE417056408D614650D16750F10AE88D4AF1），
 pyresample (8182DE417056408D614650D16750F10AE88D4AF1),
 pysolid（8182DE417056408D614650D16750F10AE88D4AF1），
 pyspectral（8182DE417056408D614650D16750F10AE88D4AF1），
 pysph（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 pystac（8182DE417056408D614650D16750F10AE88D4AF1），
 pystac-client (8182DE417056408D614650D16750F10AE88D4AF1)
 pytables（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 pytest-recording (8182DE417056408D614650D16750F10AE88D4AF1),
 python-affine (8182DE417056408D614650D16750F10AE88D4AF1)
 python-cartopy (8182DE417056408D614650D16750F10AE88D4AF1)
 python-geographiclib（8182DE417056408D614650D16750F10AE88D4AF1），
 python-geojson（8182DE417056408D614650D16750F10AE88D4AF1），
 python-geopandas (8182DE417056408D614650D16750F10AE88D4AF1),
 python-geotiepoints（8182DE417056408D614650D16750F10AE88D4AF1），
 python-hdf4 (8182DE417056408D614650D16750F10AE88D4AF1)
 python-ltfatpy (BBBD45EA818AB86FF67E7285D3E17383CFA7FF06)
 python-pint（A0B1A9F3508956130E7A425CD416AD15AC6B43FE），
 python-polsarpro (8182DE417056408D614650D16750F10AE88D4AF1),
 python-rioxarray (3E99A526F5DCC0CBBF1CEEA600BAE74B343369F1)
 python-s3fs (8182DE417056408D614650D16750F10AE88D4AF1)
 pytroll-schedule (8182DE417056408D614650D16750F10AE88D4AF1),
 吡唑坦（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 rasterio (8182DE417056408D614650D16750F10AE88D4AF1),
 remotezip (8182DE417056408D614650D16750F10AE88D4AF1),
 resampy（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 裡奧-cogeo (8182DE417056408D614650D16750F10AE88D4AF1),
 sarsen (8182DE417056408D614650D16750F10AE88D4AF1),
 satpy (8182DE417056408D614650D16750F10AE88D4AF1),
 賽特（2861257317C7AEE4F880497EC3860AC59F574E3A），
 天場（3E99A526F5DCC0CBBF1CEEA600BAE74B343369F1），
 切片器（8182DE417056408D614650D16750F10AE88D4AF1），
 snaphu (8182DE417056408D614650D16750F10AE88D4AF1),
 stac-check (8182DE417056408D614650D16750F10AE88D4AF1),
 stac-pydantic (8182DE417056408D614650D16750F10AE88D4AF1),
 stac-validator (8182DE417056408D614650D16750F10AE88D4AF1)
 stactools（8182DE417056408D614650D16750F10AE88D4AF1），
 stream-zip (8182DE417056408D614650D16750F10AE88D4AF1),
 三角形（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 trollimage（8182DE417056408D614650D16750F10AE88D4AF1），
 trollsift（8182DE417056408D614650D16750F10AE88D4AF1），
 universal-pathlib（8182DE417056408D614650D16750F10AE88D4AF1），
 usgs（8182DE417056408D614650D16750F10AE88D4AF1），
 utm（8182DE417056408D614650D16750F10AE88D4AF1），
 xarray-ceos-alos2 (8182DE417056408D614650D16750F10AE88D4AF1),
 xarray-datatree (8182DE417056408D614650D16750F10AE88D4AF1),
 xarray-eopf (8182DE417056408D614650D16750F10AE88D4AF1),
 xarray-safe-rcm (8182DE417056408D614650D16750F10AE88D4AF1)
 xarray-safe-s1 (8182DE417056408D614650D16750F10AE88D4AF1)
 xarray-sentinel（8182DE417056408D614650D16750F10AE88D4AF1），
 xcube-resampleling (8182DE417056408D614650D16750F10AE88D4AF1),
 xradarsat2（8182DE417056408D614650D16750F10AE88D4AF1），
 xsar（8182DE417056408D614650D16750F10AE88D4AF1），
 札爾（BBBD45EA818AB86FF67E7285D3E17383CFA7FF06），
 zfp (B60A1BF363DC1319FF0A8E89116852BCDF7515C0)

指紋：D4969DDC46653276591FC45D7E6C0B9EB5944CEB
UID：Arif Ali <arifali1@gmail.com>
允許：sos (7D1ACFFAD9E0806C9C4CD3925C13D6DB93052E03)

指紋：7A7D93082BD19BAFA83B7E34FE9007B8ED640421
Uid：Aryan Karamtoth <spaciouscoder78@disroot.org>
允許：笨重（F18BDC8B6C25F90AA23D5174634DC4F0687046F8），
 dynstr（8F6DE104377F3B11E741748731F3144544A1741A），
 指智 (8F6DE104377F3B11E741748731F3144544A1741A),
 hyprshade（F18BDC8B6C25F90AA23D5174634DC4F0687046F8），
 niri-companion (8F6DE104377F3B11E741748731F3144544A1741A),
 夜曲（14593BFF4A5EBF6FE0E9716EECBEDBB607B9B2BE），
 播放.it（72CE56ADD3F7AB42E50EF22BCD3A6DF75742FDB1），
 play.it-action (72CE56ADD3F7AB42E50EF22BCD3A6DF75742FDB1),
 play.it-動作冒險 (8F6DE104377F3B11E741748731F3144544A1741A),
 play.it-community（72CE56ADD3F7AB42E50EF22BCD3A6DF75742FDB1），
 play.it平台（72CE56ADD3F7AB42E50EF22BCD3A6DF75742FDB1），
 play.it-puzzle (72CE56ADD3F7AB42E50EF22BCD3A6DF75742FDB1),
 play.it-rpg (72CE56ADD3F7AB42E50EF22BCD3A6DF75742FDB1),
 play.it-strategy（72CE56ADD3F7AB42E50EF22BCD3A6DF75742FDB1），
 play.it-vv221 (72CE56ADD3F7AB42E50EF22BCD3A6DF75742FDB1),
 pybel（C63DBBEF21427CE249DBD96B061212944647A411），
 pymongo（8F6DE104377F3B11E741748731F3144544A1741A），
 吡喃糖（C63DBBEF21427CE249DBD96B061212944647A411），
 吡爾 (8F6DE104377F3B11E741748731F3144544A1741A),
 python-awkward (A095B66EE09024BEE6A2F0722A27904BD7243EDA)
 python-bioframe（A095B66EE09024BEE6A2F0722A27904BD7243EDA），
 python-boost-histogram (7E7729476D87D6F11D91ACCBC293E7B461825ACE)
 python-chevron (8F6DE104377F3B11E741748731F3144544A1741A)
 python-doubly-py-linked-list (8F6DE104377F3B11E741748731F3144544A1741A),
 python-fontfeatures（8F6DE104377F3B11E741748731F3144544A1741A），
 python-hepunits (7E7729476D87D6F11D91ACCBC293E7B461825ACE)
 python-markdownify (8F6DE104377F3B11E741748731F3144544A1741A),
 python-mpris-伺服器（F18BDC8B6C25F90AA23D5174634DC4F0687046F8），
 python-pyspoa（A095B66EE09024BEE6A2F0722A27904BD7243EDA），
 python-pytooling (7E7729476D87D6F11D91ACCBC293E7B461825ACE)
 python-resample (7E7729476D87D6F11D91ACCBC293E7B461825ACE),
 python-streamz (8F6DE104377F3B11E741748731F3144544A1741A)
 python-strenum（F18BDC8B6C25F90AA23D5174634DC4F0687046F8），
 python-syncedlyrics (F18BDC8B6C25F90AA23D5174634DC4F0687046F8),
 python-tinytag (8F6DE104377F3B11E741748731F3144544A1741A),
 python-uhi (7E7729476D87D6F11D91ACCBC293E7B461825ACE)
 python-vector (7E7729476D87D6F11D91ACCBC293E7B461825ACE)
 raylib (772292F6F7AC85FAE041D41EE5F43F9C2734F287)

指紋：439884E6862A429C290DF63B033C4CA276024834
使用者 ID：Athos Ribeiro <athos.ribeiro@canonical.com>
允許：isc-kea (1BD886F246FD490879D4E1505A09B4576DE8080E)
 mdevctl (237A54B1028728BF00EF31F4D0EB762865FC5E36),
 php-doc（237A54B1028728BF00EF31F4D0EB762865FC5E36），
 php-fig-log-test (237A54B1028728BF00EF31F4D0EB762865FC5E36)
 podman-compose (237A54B1028728BF00EF31F4D0EB762865FC5E36)

指紋：AF031CB8DFFB7DC5E1EEEB04A7C9FF063F3D2E03
Uid: Axel Wagner <axel@mathphys.fsk.uni-heidelberg.de>
允許：shellex (424E14D703E7C6D43D9D6F364E7160ED4AC8EE1D)

指紋：DC184C7074DC4FD338D86CF97E32B4D596D6F8F6
使用者 ID：Aymeric Agon-Rambosson <ricorambo@ricorambo.su>
允許：citar (DE6BA671D57D9B009CF686505EE76EE20216D2A5)
 compat-el (DE6BA671D57D9B009CF686505EE76EE20216D2A5),
 consult-el（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 davfs2 (3AFA757FAC6EA11D2FF45DF088D24287A2D898B1),
 ebib（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 eglot（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 elpa-undo-tree (DE6BA671D57D9B009CF686505EE76EE20216D2A5)
 emacs-async (DE6BA671D57D9B009CF686505EE76EE20216D2A5)
 emacs-pdf-tools (DE6BA671D57D9B009CF686505EE76EE20216D2A5)
 emacsql (DE6BA671D57D9B009CF686505EE76EE20216D2A5),
 登船（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 ggtags（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 gnuplot-mode（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 gumbo-parser（2861257317C7AEE4F880497EC3860AC59F574E3A），
 馬吉特（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 頁邊註（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 無序（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 org-roam (DE6BA671D57D9B009CF686505EE76EE20216D2A5)
 ox-texinfo-plus (DE6BA671D57D9B009CF686505EE76EE20216D2A5)
 解析比卜（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 彈丸（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 queue-el（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 彩虹分隔符號（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 spinner-el (DE6BA671D57D9B009CF686505EE76EE20216D2A5),
 無吸盤工具（9AE04D986400E3B67528F4930D442664194974E2），
 垂直（DE6BA671D57D9B009CF686505EE76EE20216D2A5），
 xml-rpc-el (DE6BA671D57D9B009CF686505EE76EE20216D2A5)

指紋：D96195E04D8045FF4160FD1728D9A6F364EB7512
Uid：Benjamin Kaduk <bjk@FreeBSD.org>
允許：krb5 (39272F04C8E560DC056CE2F3FC8D76733C86260F)
 openafs (39272F04C8E560DC056CE2F3FC8D76733C86260F)

指紋：480C30BEF10685220CBFD5EE87157C329108F09E
使用者 ID：Blake Lee <blake@volian.org>
允許：nala (BB45B0B3FF561BDBD45EE8A9B35B49EA5D563EFE)
 rust-rust-apt (14593BFF4A5EBF6FE0E9716EECBEDBB607B9B2BE)

指紋：BA60BC20F37E59444D6D25001365720913D2F22D
Uid：Boian Bonev <bbonev@ipacct.com>
允許：bpfmon (FD9CE2D8D7754B78AB279BBD2C3B436FEAC68101)
 複雜度（2861257317C7AEE4F880497EC3860AC59F574E3A），
 dhcpdump (FD9CE2D8D7754B78AB279BBD2C3B436FEAC68101)
 DHCPping（2861257317C7AEE4F880497EC3860AC59F574E3A），
 伽穆（2861257317C7AEE4F880497EC3860AC59F574E3A），
 GPSD（2861257317C7AEE4F880497EC3860AC59F574E3A），
 iotop-c (610B28B55CFCFE45EA1B563B3116BA5E9FFA69A3)
 vfu（FD9CE2D8D7754B78AB279BBD2C3B436FEAC68101），
 yascreen (FD9CE2D8D7754B78AB279BBD2C3B436FEAC68101)

指紋：FB39DE61869F49D5CCC83AE0D53A15D983A10B94
Uid：Braulio Henrique Marques Souto <braulio@disroot.org>
允許：golang-github-aybabtme-rgbterm (A095B66EE09024BEE6A2F0722A27904BD7243EDA)
 golang-github-thoas-go-funk (A095B66EE09024BEE6A2F0722A27904BD7243EDA),
 md2term (357DCB0EEC95A01AEBA1F0D2DE63B9C704EBE9EF),
 mutt-wizard（B522F39159DA07DD39DC0B11F4BAAA80DB28BA4C），
 ytfzf (357DCB0EEC95A01AEBA1F0D2DE63B9C704EBE9EF)

指紋：258E9BF2AB5576F2C5C0949A2C376EADE7855D90
Uid：Carl Keinath <carl.keinath@gmail.com>
允許：釉料（D3F0E02EC45A938E1D67229EC43496655925B604），
 hyprlauncher（12E0D09DFB3FF7F759D36ED0FBD5225B588752A1），
 hyprpicker（12E0D09DFB3FF7F759D36ED0FBD5225B588752A1），
 neovim-autopairs (14593BFF4A5EBF6FE0E9716EECBEDBB607B9B2BE),
 neovim-gitsigns（14593BFF4A5EBF6FE0E9716EECBEDBB607B9B2BE），
 neovim-indent-blankline (14593BFF4A5EB(2861257317
