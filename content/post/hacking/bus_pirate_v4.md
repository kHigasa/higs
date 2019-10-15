---
title: "Bus Pirate v4の回路基盤を確認する"
date: 2019-10-15T22:06:14+09:00
categories:
- information security
- IoT hacking
tags:
- information security
- physics
- electronic circuit
keywords:
- Bus Pirate v4
thumbnailImage: images/bus_pirate_v4.jpg
draft: true
---

PC-電子デバイス間のデバッグ・解析ツールである[```Bus Pirate v4```](https://www.seeedstudio.com/Bus-Pirate-v4.html)の基盤を解析し, その挙動を回路基盤より見ることが本稿での狙いである.

<!--more-->

*ファームウェアへのアプローチではないため, そこを確認したい方は[GitHubのリポジトリ](https://github.com/BusPirate/Bus_Pirate)でも参照してほしい.

<!--toc-->

# Schematic and PCB (回路図とプリント回路版)

先に回路図を示す. 別タブ表示や拡大等しっかり見るには工夫を要するだろうが, 興味ある方はぜひ参照してほしい.
![bus_pirate_v4a_schematic](images/BusPirate-v4a.sch.png)
*reference1より

### references
1. [Bus Pirate v4 design overview](http://dangerousprototypes.com/docs/Bus_Pirate_v4_design_overview)
