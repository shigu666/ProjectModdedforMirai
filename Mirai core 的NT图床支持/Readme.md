# 使mirai支持新NT图床方法

## 1.将`mirai-core-all-2.17.0-all.jar`和`mirai-core-all-2.17.0-all.jar.sha1`放入`libs`文件夹
## 2.修改`config.json`中的内容，将
```json
    "net.mamoe:mirai-core-all": {
      "channel": "maven-stable",
      "version": "2.16.0",
      "type": "libs",
      "versionLocked": false
    }
```
## 修改为
```json
    "net.mamoe:mirai-core-all": {
      "channel": "maven-stable",
      "version": "2.17.0",
      "type": "libs",
      "versionLocked": true
    }
```
修改来源[mamoe/mirai/Pull request #2860](https://github.com/mamoe/mirai/pull/2860)，文件来自Actions构建[mamoe/mirai/Build #5103](https://github.com/mamoe/mirai/actions/runs/10643417415)