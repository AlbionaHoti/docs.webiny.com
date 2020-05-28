---
id: app
title: App Plugins Reference
sidebar_label: App
---

### [`admin-file-manager-file-type`](/docs/webiny-apps/security/development/plugin-reference/app#admin-file-manager-file-type)

#### Summary

// Use a picture to show the `admin-file-manager-file-type`

#### Type

```ts
type AdminFileManagerFileTypePlugin = Plugin & {
    type: "admin-file-manager-file-type";
    types?: string[];
    render({ file }): React.ReactNode;
    fileDetails?: {
        actions: Array<React.FunctionComponent | React.Component>;
    };
};
```

#### Example

```ts
    {
        name: "file-manager-file-type-default",
        type: "admin-file-manager-file-type",
        render() {
            return (
                <div className={style.centering}>
                    <FileIcon />
                </div>
            );
        }
    }
```
