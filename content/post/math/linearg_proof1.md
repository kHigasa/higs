---
title: "正則なn次正方行列Aの余因子行列の行列式が|A|のn-1乗であることの証明"
date: 2020-04-06T23:26:43+09:00
categories:
- Linear Algebra
- proof
tags:
- Linear Algebra
- proof
keywords:
- determinant
- adjoint matrix
thumbnailImage: https://1.bp.blogspot.com/-u4tcj_Qm67U/Vtd-y7iwdNI/AAAAAAAA4TI/seWxtFeOte0/s800/sotsugyou_dai2_button.png
---

行列式のn乗を求めて解答する問題があったが, その際設問の誘導に従って使用した式変形が有用であったのでここにその証明を付しておく.

<!--more-->

<!--toc-->

# 証明する式
if
$$
\mathrm{det}A\neq0
$$
then
$$
\mathrm{det}(\mathrm{adj}A) = (\mathrm{det}A)^{n-1}
$$
ここで, $\mathrm{det}A$(ディターミナントエー)は$A$の行列式, $\mathrm{adj}A$(アジョイントエー)は$A$の余因子行列を表す.

## 参考
このYouTube動画をそのまま踏襲したのでここに予め記しておきます.
{{< youtube 3MYHz2z0Cs0>}}

## *Proof.*
まず正則なn次正方行列$A$の余因子行列に対して,
$$
A\cdot\mathrm{adj}A=\mathrm{adj}A{\cdot}A=\mathrm{det}A{\cdot}I_n
$$
が成り立つ(ここで$I_n$はn次単位行列を表す). これは行列式の行と列に関する余因子展開により速やかに示される主張である. ここで証明を付すことはしないが, 入門程度の教科書にて一度証明を追った後は覚えておくと良い.

次に上式の行列式を取ると,
$$
\mathrm{det}(A\cdot\mathrm{adj}A)=\mathrm{det}A{\cdot}\mathrm{det}(\mathrm{adj}A)(\because乗法定理^{*1})
$$
$$
=\mathrm{det}(\mathrm{det}A{\cdot}I_n)=
\mathrm{det}\left(
  \begin{array}{cccc}
    \mathrm{det}A & 0 & \ldots & 0 \cr
    0 & \mathrm{det}A & \ldots & 0 \cr
    \vdots & \vdots & \ddots & \vdots \cr
    0 & 0 & \ldots & \mathrm{det}A
  \end{array}
\right)=
(\mathrm{det}A)^n
$$
$^{*1}$2つのn次正方行列の積の行列式$\mathrm{det}AB$は各行列の行列式の積$\mathrm{det}A\cdot\mathrm{det}B$に等しい(行列式の交代性と多重線形性による帰結 [1]).

となる. 最後に両辺を$\mathrm{det}A(\neq0)$で割って求める式
$$
\mathrm{det}(\mathrm{adj}A) = (\mathrm{det}A)^{n-1}
$$
を得る.<div style="text-align: right">$\Box$</div>

### References
1. 斉藤正彦 (2014). 線形代数学 東京図書

