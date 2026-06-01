# Nero-dalamud

卫月 / Dalamud 第三方插件仓库。

仓库地址：

```text
https://raw.githubusercontent.com/Nero0421/Nero-dalamud/main/repo.json
```

当前包含：

- AoAoEnergy / 嗷嗷有劲，API 15

## 添加插件

后续新增插件时，把插件 zip 放到 `plugins/<InternalName>/`，然后在 `repo.json` 的数组里追加一个插件对象。`InternalName` 必须和插件 DLL/manifest 保持一致，`AssemblyVersion` 要和 zip 内插件版本一致，`DalamudApiLevel` 要和当前卫月 API 匹配。