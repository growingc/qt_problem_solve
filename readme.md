2023.7.26
使用stackview加载一个A.qml文件时，报错 xx is not a type. 其中xx指的是自定义的B.qml, 在A.qml 中被使用。
前提：A、B都在同一个文件夹，qrc配置没有问题。
解决：stackview加载A.qml时路径问题，需要按照qrc中写的一致，特别是prefix="/" 这个斜杠不能少，stackView.push("qrc:/qml/homepage/HomePage.qml")
