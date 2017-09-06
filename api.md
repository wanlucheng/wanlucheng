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
### 3. /article/getArticleList
### 4. /article/getArticleListPlug
### 5. /article/getArticleDetail
