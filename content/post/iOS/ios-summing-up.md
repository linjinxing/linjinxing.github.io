+++
banner = "banners/placeholder.png"
categories = ["iOS"]
date = "2015-12-19T13:39:46+02:00"
tags = ["总结","iOS"]
title = "iOS总结"
+++


1，遇到XCode解析代码特别慢，SourceKitService占用cpu率很高。使用xcodebuild -workspace MiaoleGB.xcworkspace -scheme MiaoleGB clean build 2>&1 |egrep "\d.\dms"|sort -nr > culprits.txt 命令查收出分析比较慢的代码：[(1...10).map({String($0) + " 室"}), (0...5).map({String($0) + " 厅"}), (0...5).map({String($0) + " 卫"})]

