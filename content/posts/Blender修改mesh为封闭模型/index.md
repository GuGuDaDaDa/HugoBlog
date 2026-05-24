+++

title = 'Blender修改mesh为封闭模型'

subtitle = '使用Blender手动修改mesh为封闭模型(watertight)'

date = 2026-05-23T09:00:00+08:00

lastmod = ''

featured = false

description = ''

categories = ['学习']

tags = ['研究生活']

cover = 'cover.jpg'

draft = false

+++

## 前言

之前我一直使用Meshlab的fill holes自动修补mesh，但有些模型自动修补效果不好，需要额外手动添加三角面。

## Fill Holes

使用blender打开模型，按下`Tab`进入编辑模式，选择`Edge Mode`,按住`Shift`选择需要修补的部分，然后按`F`即可自动填充。

![编辑模式](https://static.246266.xyz/i/2024/05/27/665448f027e84.png#vwid=525&vhei=147)

![选择边](https://static.246266.xyz/i/2024/05/27/6654495569df8.png#vwid=1048&vhei=210)

## 转化为三角面

这样新添加的面可能不是三角面，需要将其修改为三角面，进入编辑模式，选择`Face Mode`,按下`Ctrl + T`自动转化为三角面。

另外，自动修补出的三角面部分法向量可能会相反，可以在此模式下，进行`Mesh->Normal->Flip`进行反转。

![反转法向量](https://static.246266.xyz/i/2024/05/27/66544def69236.png#vwid=800&vhei=379)


{{< refers   title="参考">}}
{{< refer desc="Blender Tutorial: Different Ways to Fill Holes" url="https://www.youtube.com/watch?v=YliK6XkLhe" >}}
{{< refer desc="面三角化" url="https://docs.blender.org/manual/zh-hans/4.0/modeling/meshes/editing/face/triangulate_faces.html" >}}
{{< refer desc="翻转" url="https://docs.blender.org/manual/zh-hans/3.1/modeling/meshes/editing/mesh/normals.html" >}}
{{< refer desc="封面图" url="https://artsandculture.google.com/asset/komposition-mit-rot-blau-und-gelb/5QG2Fm_LGUWAHA?hl=zh-CN" >}}
{{< /refers >}}