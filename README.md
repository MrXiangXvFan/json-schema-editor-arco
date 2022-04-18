# Json Schema 可视化编辑器（Arco）

## 快速开始

```
# 开发
npm run dev

# 构建
npm run build

# 发布前预览
npm run prepublishOnly && arco preview

# 发布至物料平台（需先发布 NPM 包）
arco sync
```

## 示例

```typescript jsx
import JsonSchemaEditor from '@quiet-front-end/json-schema-editor-arco';
import '@quiet-front-end/json-schema-editor-arco/dist/css/index.css';
import { useEffect } from 'react';

export default (props: ApiEditProps) => {

  const [jsonData, setJsonData] = useEffect({});

  return (
    <JsonSchemaEditor
      mock={true}
      data={jsonData}
      onChange={(data) => {
        setJsonData(data);
      }}
    />
  )
}
```

![示例](./image/img.png)

