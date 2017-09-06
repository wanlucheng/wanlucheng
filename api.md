### 1. 获取所有分类列表

- /article/getTypeList
- method: get

#### 请求参数

| key | type | desc |
|-----|------|------|
| - | - | - |

#### 响应参数

| key | type | desc |
|-----|------|------|
| type_id | int | 类型ID |
| name | string | 类型名称 |

``` json 
{
  "code": 0,
  "data": {
    "list": [
      {
        "type_id": 1,
        "name": "公告"
      },
      {
        "type_id": 2,
        "name": "新闻"
      },
      {
        "type_id": 3,
        "name": "教程"
      }
    ]
  },
  "msg": ""
}
```

### 2. 获取所有标签列表

- /article/getTagList
- method: get

#### 请求参数

| key | type | desc |
|-----|------|------|
| - | - | - |

#### 响应参数

| key | type | desc |
|-----|------|------|
| tag_id | int | 标签ID |
| name | string | 标签名称 |

``` json 
{
  "code": 0,
  "data": {
    "list": [
      {
        "tag_id": 1,
        "name": "比特币"
      }
    ]
  },
  "msg": ""
}
```
### 3. 获取文章列表
- /article/getArticleList
- method: get

#### 请求参数

| key | type | desc |
|-----|------|------|
| key | string | 查找的关键字 |
| value | string | 查找的匹配值 |
| start | int | 查找的起始位置(按文章创建时间倒序排序) |
| count | int | 文章个数 |

  /article/getArticleList?key=分类&value=公告&start=0&count=10

#### 响应参数

| key | type | desc |
|-----|------|------|
| article_id | int | 文章ID |
| type_id | int | 文章类型ID |
| type_name | string | 文章类型名称 |
| title | string | 文章标题 |

``` json 
{
  "code": 0,
  "data": {
    "list": [
      {
        "article_id": 1,
        "type_id": 1,
        "type_name": "公告",
        "title": "测试'"
      }
    ]
  },
  "msg": ""
}
```

### 4. /article/getArticleListPlug
### 5. /article/getArticleDetail
