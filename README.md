# MPF UI Components

Qt Modular Plugin Framework - UI Components Library (QML)

## 概述

提供统一风格的 QML 组件，用于构建一致的用户界面。

## 组件列表

| 组件 | 说明 |
|------|------|
| `MPFCard` | 卡片容器 |
| `MPFButton` | 按钮 |
| `MPFDialog` | 对话框 |
| `MPFTextField` | 输入框 |
| `MPFIconButton` | 图标按钮 |
| `MPFLoadingIndicator` | 加载指示器 |
| `StatusBadge` | 状态徽章 |

## 依赖

- Qt 6.5+ (Core, Gui, Qml, Quick)

## 安装

### 从源码构建

```bash
export QT_DIR=/path/to/qt6
export MPF_SDK=/path/to/mpf-sdk

cmake -B build -G Ninja \
    -DCMAKE_PREFIX_PATH="$QT_DIR" \
    -DCMAKE_INSTALL_PREFIX="$MPF_SDK"
cmake --build build
cmake --install build
```

## 使用

```qml
import MPF.Components 1.0

MPFCard {
    title: "My Card"
    
    MPFButton {
        text: "Click Me"
        onClicked: console.log("Clicked!")
    }
}
```

## 许可证

MIT License
