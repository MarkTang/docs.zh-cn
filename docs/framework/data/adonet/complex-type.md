---
title: Complex Type — 复杂类型
ms.date: 03/30/2017
ms.assetid: 63efbd23-11d4-4871-bc88-ad01b9837553
ms.openlocfilehash: 8daeac8309434b3c4e090d8e75f2de02d63e8b11
ms.sourcegitcommit: 11f11ca6cefe555972b3a5c99729d1a7523d8f50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2018
ms.locfileid: "32756808"
---
# <a name="complex-type"></a>Complex Type — 复杂类型
A*复杂类型*是用于定义上的丰富的结构化属性的模板[实体类型](../../../../docs/framework/data/adonet/entity-type.md)或其他复杂类型。 每个模板都包含以下内容：  
  
-   唯一名称。 （必需）  
  
    > [!NOTE]
    >  复杂类型的名称不能与同一命名空间中的实体类型的名称相同。  
  
-   形式的一个或多个数据[属性](../../../../docs/framework/data/adonet/property.md)。 （可选）。  
  
    > [!NOTE]
    >  复杂类型的属性可以是另一个复杂类型。  
  
 复杂类型与实体类型相似，因为复杂类型可以以基元类型属性或其他复杂类型的形式携带数据负载。 但是，在复杂类型与实体类型之间仍存在着一些重要区别：  
  
-   复杂类型没有标识，因此不能独立存在。 复杂类型只能作为实体类型或其他复杂类型的属性而存在。  
  
-   复杂类型不能参与[关联](../../../../docs/framework/data/adonet/association-type.md)。 关联的任一端都不可以是复杂类型，因此[导航属性](../../../../docs/framework/data/adonet/navigation-property.md)不能对复杂类型定义。  
  
## <a name="example"></a>示例  
 [ADO.NET 实体框架](../../../../docs/framework/data/adonet/ef/index.md)使用域特定语言 (DSL) 称为概念架构定义语言 ([CSDL](../../../../docs/framework/data/adonet/ef/language-reference/csdl-specification.md)) 来定义概念模型。 下面的 CSDL 定义了一个复杂类型 Address，它具有基元类型属性 `StreetAddress`、`City`、`StateOrProvince`、`Country` 和 `PostalCode`。  
  
 [!code-xml[EDM_Example_Model#ComplexTypeExample](../../../../samples/snippets/xml/VS_Snippets_Data/edm_example_model/xml/books2.edmx#complextypeexample)]  
  
 若要将复杂类型 `Address`（如上所示）定义为某个实体类型的属性，必须在实体类型定义中声明该属性类型。 下面的 CSDL 将 `Address` 属性声明为实体类型 (Publisher) 的复杂类型：  
  
 [!code-xml[EDM_Example_Model#EntityWithComplexType](../../../../samples/snippets/xml/VS_Snippets_Data/edm_example_model/xml/books3.edmx#entitywithcomplextype)]  
  
## <a name="see-also"></a>请参阅  
 [实体数据模型关键概念](../../../../docs/framework/data/adonet/entity-data-model-key-concepts.md)  
 [实体数据模型](../../../../docs/framework/data/adonet/entity-data-model.md)
