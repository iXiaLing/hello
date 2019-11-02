[Sourcetree 官网](https://www.sourcetreeapp.com/)

**旧版**只需要添加 *accounts.json* 文件就能实现免注册登录

**新版**需要添加 *accounts.json* 文件和添加 *user.config* 字段。

### 创建accounts.json文件

文件路径：```%LocalAppData%\Atlassian\SourceTree\accounts.json```

accounts.json内容
```json
[
  {
    "$id": "1",
    "$type": "SourceTree.Api.Host.Identity.Model.IdentityAccount, SourceTree.Api.Host.Identity",
    "Authenticate": true,
    "HostInstance": {
      "$id": "2",
      "$type": "SourceTree.Host.Atlassianaccount.AtlassianAccountInstance, SourceTree.Host.AtlassianAccount",
      "Host": {
        "$id": "3",
        "$type": "SourceTree.Host.Atlassianaccount.AtlassianAccountHost, SourceTree.Host.AtlassianAccount",
        "Id": "atlassian account"
      },
      "BaseUrl": "https://id.atlassian.com/"
    },
    "Credentials": {
      "$id": "4",
      "$type": "SourceTree.Model.BasicAuthCredentials, SourceTree.Api.Account",
      "Username": "",
      "Email": null
    },
    "IsDefault": false
  }
]
```

### 修改user.config 配置
文件路径：```%LocalAppData%\Atlassian\SourceTree.exe_Url_xxxxxxxxxx\3.1.2.3027\user.config```

其中的*xxxxxxxxxx\3.1.2.3027*需要根据实际情况调整，记事本打开 user.config，在 <SourceTree.Properties.Settings> 添加以下内容并保存即可。
```xml
<setting name="AgreedToEULAVersion" serializeAs="String">
	<value>20160201</value>
</setting>
```