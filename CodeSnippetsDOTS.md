# Unity DOTS snippets

`Preferences/Configure User Snipptes` -> Select c# as a language -> Paste snippets in the opened file

```
{
	// The unity.com.entities code snippets for creation
	"Authoring":
	{
		"prefix": "author",
		"body":[
			"using UnityEngine;",
			"",
			"using Unity.Entities;",
			"using Unity.Mathematics;",
			"",
			"public class ${1:Name}Authoring : MonoBehaviour",
			"{",
			"    $0",
			"}",
			"",
			"class ${1:Name}Baker : Baker<${1:Name}Authoring>",
			"{",
			"    public override void Bake(${1:Name}Authoring authoring)",
			"    {",
			"        ",
			"    }",
			"}"
		],
		"description": "Make an authoring monobehaviour and baker in ECS Unity"
	},

	"System": {
		"prefix": "system",
		"body": [
			"using Unity.Entities;",
			"using Unity.Mathematics;",
			"using Unity.Transforms;",
			"",
			"partial struct ${1:Name}System : ISystem\n{",
			"    public void OnUpdate(ref SystemState state)",
			"    {",
			"        $0",
			"    }",
			"}"
		],
		"description": "Make a system in ECS Unity"
	},

	"Component": {
		"prefix": "component",
		"body": [
			"using Unity.Entities;",
			"using Unity.Mathematics;",
			"",
			"public struct ${1:Name} : IComponentData\n{",
			"    $0",
			"}"
		],
		"description": "Make a component in ECS Unity"
	}
}
```
