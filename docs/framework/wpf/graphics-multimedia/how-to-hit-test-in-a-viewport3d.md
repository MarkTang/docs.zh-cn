---
title: 如何：在 Viewport3D 中进行命中测试
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- 3-D visuals [WPF], hit-testing for
- hit tests [WPF], for 3-D visuals
- Viewport3D [WPF]
ms.assetid: 42bfbd99-c7c6-43f1-940b-90448faa412e
ms.openlocfilehash: ab097e11490fda7a8e3b23c8749204f091271919
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
ms.locfileid: "33559653"
---
# <a name="how-to-hit-test-in-a-viewport3d"></a>如何：在 Viewport3D 中进行命中测试
此示例演示如何执行命中测试的 3D 视觉对象中<xref:System.Windows.Controls.Viewport3D>。  
  
 因为<xref:System.Windows.Media.VisualTreeHelper.HitTest%2A>返回 2D 和 3D 信息，可以循环访问测试结果，以仅读取三维结果。  
  
 [!code-csharp[HitTest3D#HitTest3D3DN4](../../../../samples/snippets/csharp/VS_Snippets_Wpf/HitTest3D/CSharp/Window1.xaml.cs#hittest3d3dn4)]
 [!code-vb[HitTest3D#HitTest3D3DN4](../../../../samples/snippets/visualbasic/VS_Snippets_Wpf/HitTest3D/visualbasic/window1.xaml.vb#hittest3d3dn4)]  
  
 <xref:System.Windows.Media.HitTestResultBehavior>下面的代码中确定如何处理命中的测试结果。  `UpdateResultInfo` 和`UpdateMaterial`本地定义的方法。  
  
 [!code-csharp[HitTest3D#HitTest3D3DN5](../../../../samples/snippets/csharp/VS_Snippets_Wpf/HitTest3D/CSharp/Window1.xaml.cs#hittest3d3dn5)]
 [!code-vb[HitTest3D#HitTest3D3DN5](../../../../samples/snippets/visualbasic/VS_Snippets_Wpf/HitTest3D/visualbasic/window1.xaml.vb#hittest3d3dn5)]  
  
## <a name="see-also"></a>请参阅  
 [三维命中测试示例](http://go.microsoft.com/fwlink/?LinkID=159959)
