# Nero-dalamud

卫月 / Dalamud 第三方插件仓库。

## 仓库地址

```text
https://raw.githubusercontent.com/Nero0421/Nero-dalamud/main/repo.json
```

## 当前包含

- AoAoEnergy / 嗷嗷有劲，API 15
- Casexile / 命令大小写修正，API 15
  - 让斜杠命令不区分大小写。输入 `/ND`、`/NEKO` 这类大小写不一致的命令时，会自动修正命令头，后面的参数保持原样。

## 添加插件

后续新增插件时，把插件 zip 放到 `plugins/<InternalName>/`，然后在 `repo.json` 和 `pluginmaster.json` 的数组里追加插件对象。

需要注意：

- `InternalName` 必须和插件 DLL / manifest 保持一致。
- `AssemblyVersion` 必须和 zip 内插件版本一致。
- `DalamudApiLevel` 必须和当前卫月 API 匹配。
- `DownloadLinkInstall` 和 `DownloadLinkUpdate` 使用 `raw.githubusercontent.com` 链接。
