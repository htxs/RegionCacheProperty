## 简介

RegionCacheProperty 项目旨在收集全面的国内配送地址库。曾试图在网上找已有的地址库，发现部分地址库不全面，无法保证及时更新。本人业余时间通过导出淘宝客户端的地址库文件，并整理缺失的城市或地区。尝试（埋坑）不定时更新淘宝的配送地址库，所以开了这个项目。也希望有兴趣的朋友一起维护这个地址库。

当前版本的配送地址库来自淘宝 iPhone 客户端 5.3.2（1071612）版本，截至最新时间为2015年8月24日的最新数据。

`RegionCacheProperty_IncludeForeign.plist` 文件包含了海外的国家列表。但考虑到国内开发者需求，有时并不需要海外国家，所以整理了一份不包含海外国家的列表 `RegionCacheProperty_NotIncludeForeign.plist`

两个 .plist 文件已经转换为 XML 格式，方便读取和修改。建议使用到项目中时，将 XML 格式转换为二进制文件，以减少文件占用大小。可以使用以下2个命令在 XML 格式和二进制文件格式之间进行转换。

```bash
# 将 plist 文件转换为二进制格式
$ plutil -convert binary1 RegionCacheProperty_IncludeForeign.plist
```

```bash
# 将 plist 文件转换为 XML 格式
$ plutil -convert xml1 RegionCacheProperty_IncludeForeign.plist
```

## License

RegionCacheProperty is available under the MIT license. See the LICENSE file for more info.